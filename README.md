Readme · MD
Detection of Lumbar Spondylolisthesis from X-ray Images using Deep Learning

A deep learning system that detects and grades lumbar spondylolisthesis — a condition where a vertebra slips forward relative to the one below it — directly from spinal X-ray images. The pipeline uses a modified U-Net architecture for vertebral segmentation, automatically calculates the percentage of vertebral slip, and classifies the result into a standard severity grade.

Overview

Diagnosing spondylolisthesis traditionally requires a radiologist to manually measure vertebral displacement on an X-ray. This project automates that process end-to-end:

Takes a lumbar spine X-ray as input
Segments individual vertebrae using a CNN-based U-Net model
Calculates the percentage slip between adjacent vertebrae
Assigns a severity grade based on the measured slip
Generates an automated report through a simple web interface
Features
Automated vertebral segmentation using a modified U-Net architecture
Percentage slip calculation based on segmented vertebral boundaries
Severity grading mapped from the calculated slip percentage
Web-based interface for image upload and report generation
MySQL-backed storage for patient/report records
