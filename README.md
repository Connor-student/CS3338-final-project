1 Project Overview
The JPL Lunar Detection Pipeline is NASA’s Lunar Reconnaissance Orbiter Camera
(LROC) captures high-resolution imagery of the lunar surface, generating vast quantities of
data that require analysis to identify scientifically significant geological features. Manual
review of this imagery is time-intensive and limits the pace at which researchers can survey
the Moon for features of interest such as craters, boulders, slopes, and other formations
critical to understanding lunar geology and planning future exploration missions. Automated
feature detection addresses this bottleneck by enabling rapid, systematic analysis of LROC
imagery, allowing scientists to focus their expertise on interpreting results rather than initial
identification tasks.


2 Objectives
The machine learning pipeline processes raw LROC imagery through preprocessing stages
that normalize image data and prepare it for model inference. YOLOv11 and Detectron2
models execute feature detection, generating bounding boxes, classification labels, and con-
fidence scores for identified objects. The pipeline handles NASA’s specialized image formats
and accommodates the unique challenges of lunar imagery such as varying illumination an-
gles, shadowing effects, and complex terrain topology. Post-processing stages filter results
based on confidence thresholds and eliminate duplicate detections. The output includes an-
notated imagery with detected features highlighted, CSV files containing feature metadata
(coordinates, dimensions, classifications), and performance metrics for model evaluation.
This automated workflow significantly accelerates the analysis process compared to manual
methods, enabling systematic surveys of large lunar regions and rapid identification of areas
warranting further investigation for mission planning or scientific study.


3 Project Goals and Motivation

3.1 Why This Project Is Needed
Modern lunar missions and research programs generate massive quantities of image data.
Manual inspection of these datasets is time-consuming, expensive, and prone to inconsis-
tency.
The JPL Lunar Detection Pipeline addresses these challenges by:
• Increasing processing speed
• Improving detection relabilty
• Supporting large scientific workflows
• Creating a data management and reporting system

3.2 Key Goals
• Improve efficiency in lunar object analysis and processing
• To implement machine learning workflows
• Provide controls for collaborative research
• Support the growing planetary image analysis
• Making a simple dashboard that give users stress free movement in the system


Features include:
• A dashboard that will show project management
• A area for data upload and check is its acceptable
• Pipeline settings
• Status checking
• Showing results reports


3.3 Processing Layer
• Data gathering and analyze
• Image processing
• Machine learning capabilties
• Results gathering and projection


3.4 Data and Storage Layer
Stores:
• Raw imagery
• Metadata
• Processed outputs
• Audit logs
• Reports and artifacts


4 Repository Information

4.1 Jira Project Link
https://cs3338-02-group-10.atlassian.net/jira/software/projects/CFPK/list/
?filter=allissues&jql=project+%3D+%22CFPK%22+ORDER+BY+created+DESC&
atlOrigin=eyJpIjoiNDFmN2VjYTFhZDdmNDY4MTg2ZjFlMTA3YTUyZWRkMDQiLCJwIjoiaiJ9


5 Installation and Setup

5.1 System Requirements
• YOLOv11
• Detectron2 (Mask R-CNN)
• PyTorch
• Python 3.10+
• Git
• Docker (optional)
• Linux, macOS, or Windows

5.2 Clone the Repository
git clone https://github.com/Connor-student/CS3338-final-project

5.3 Create a Virtual Environment
python -m venv venv
Activate environment:
# Windows
venv\Scripts\activate
# Linux / macOS
source venv/bin/activate

5.4 Install Dependencies
pip install -r requirements.txt

5.5 Run the Application
python app.py


6 How can users access the system

1. Open the web application in a browser.
2. Authenticate using organizational credentials.
3. Upload lunar image datasets or metadata.
4. Configure processing settings.
5. Start the lunar detection pipeline.
6. Monitor processing progress in real time.
7. Review and export generated results.


6.1 Access Roles
Administrator have full system access and configuration.
Data Scientists or Analysts can run pipelines and analyze results.
Viewers or Collaborators can view reports and limited datasets


7 Pipeline Workflow Summary
1. User can upload the image data
2. The System will check the incoming data for any errors
3. The System will preprocess the data
4. Detection system will analyze the data
5. Results will be safely stored
6. Reports are generated for export


8 Group10
• Connor Moy
• Kevin Mendoza
• George Malanche
• Ricky Chao


9 Reference
This is the link to Ascent JPL Lunar Detection Pipeline project info.
https://ascent.cysun.org/project/project/view/239
