# FTHformer-CMCG-YOLOv11
Official implementation of FTHformer-CMCG-YOLOv11 for transmission tower image restoration and defect detection under complex degraded imaging conditions.
# Overview
UAV-based transmission tower inspection is often affected by adverse imaging conditions, such as haze, rain streaks, snow, raindrops, and blur, which degrade image quality and reduce defect detection accuracy.
This repository provides the implementation of "FTHformer-CMCG-YOLOv11", a sequential image restoration–detection framework that integrates "FTHformer" for degraded image restoration and "CMCG-YOLOv11" for transmission tower defect detection.
The framework is designed to improve defect recognition from degraded UAV images under multiple adverse imaging conditions.
# Framework
The complete processing pipeline is:
Degraeded image        
      ↓       
FTHformer Image Restoration       
      ↓ 
Restored Image 
      ↓
CMCG-YOLOv11 defect detection
      ↓
Defect category and bounding box
