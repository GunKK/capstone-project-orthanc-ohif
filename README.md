
# Docker Compose File for OHIF with ORTHANC

## OHIF Viewer: is an open source, web-based, medical imaging platform.

## Orthanc: Its free and open-source, lightweight DICOM server for medical imaging.

* Create new docker network **dicom-network**
```
docker network create dicom-network 
```

* Clone This Repo
```
git clone https://github.com/GunKK/capstone-project-orthanc-ohif.git
```
```
cd ohif-orthanc
docker-compose up -d
```

It will also create a new /bridge-network/ pacs.

* Access OHIF and Orthanc


1. To access **OHIF** go to address `http://server-ip:3000`.
2. To access **ORTHANC** webpage go to address `http://server-ip:8042`

Default Username is `nduchau` & password is `nduchau`


*** Import DICOM Studies
1. You can directly Import DICOM files or Folder from OHIF.
2. If you have file locally install httplib2 with pip **python ImportDicomFiles.py localhost 8042 /path/to/input/dir**
