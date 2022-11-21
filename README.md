# Create-mask-realtime-use-Yolov7


Use yolov7 to detection object and segmentation it.



Dowload model train yolov7-mask:



https://github.com/WongKinYiu/yolov7/releases


Create folder 'anh' through all of file on it


Create without mask about file:


python segment2.py 


Create mask about file:


python segment2.py --nolabel --nobbox --threshhold


Create mask about realtime:


python segment2.py --source 0 --nolabel --nobbox --threshhold


Create mask about realtime to choose object


python segment2.py --source 0 --nolabel --nobbox --threshhold --mask_choose object


Ex: python segment2.py --source 0 --nolabel --nobbox --threshhold --mask_choose person


Create mask about realtime to delete object unwant and still all object you want


python segment2.py --source 0 --nolabel --nobbox --threshhold --mask_del object


Ex: python segment2.py --source 0 --nolabel --nobbox --threshhold --mask_del person
