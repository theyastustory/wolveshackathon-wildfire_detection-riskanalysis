# wolveshackathon-wildfire_detection-riskanalysis
## STAGE 1
## Fire Detection
After recieving Snapshots from Video feed, It is fed into the first model which evaluates if a fire is present or not 
## 
amazon_ec2_link: http://ec2-44-202-219-114.compute-1.amazonaws.com/
### INPUT:
![](https://github.com/theyastustory/wolveshackathon-wildfire_detection-riskanalysis/blob/main/Screenshot%20(467).png)
### OUTPUT:
![](https://github.com/theyastustory/wolveshackathon-wildfire_detection-riskanalysis/blob/main/Screenshot%20(468).png)

If Absent , the next image is evaluated
## 
If Present, we move to stage 2

## STAGE 2
## Risk Analysis
In risk analysis part we took the remote sensing data and we are preprocessing that to train the model. The data includes wind speed, temprature, specific humidity, Elevation, Wind direction, Vegetation, previous days mask and future mask, etc. there are total of 12 feautres chanells into the data.
Our model takes this data into batches and predict next days mask which is for the fire where it can spread or shrink.
