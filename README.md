# Log_fliting_API

A new API based on Python with supporting functions that enable people to create useful and simple scripts that automate event log filtering. 

## Introduction
Processes are running everywhere, and their number is rapidly increasing. The definition of a process is a series of progressive and interdependent steps by which an objective is attained. Many organizations (such as schools, companies, government agencies, universities, etc.) now use information technology systems to support Business Processes. We call a list of events recorded during the operation of information systems an event log. To better analyze these event logs, we will use the technology called Process Mining (PM).  
<br>
Unfortunately, event logs from Information Systems are usually not handled directly out-of-the-box by process mining tools. To be effective, all PM approaches include a log filtering step to clean and simplify the event logs before feeding them to mining algorithms and process visualization engines. A recent thesis proposed a new API with supporting functions that enable people to create useful and simple scripts that automate event log filtering. Below is expected to be completed APIs:   
<br>
<img src="https://github.com/Dwightu/Log_fliting_API/blob/main/api-demo.png" width="1000px">

## Objectives
- A new Python API for log filtering. This will be implemented by selecting existing libraries to support these functions, as well as developing the missing ones.
- Checking the performance of that library compared to the R-based one
- Integrating this to a popular open-source Process Mining tool written in Python (PM4PY)

## Usage
1. pip/pip3 install notebook
2. git clone https://github.com/Dwightu/Log_fliting_API.git
3. Open jupyternotebook and Run SampleScript2.r file. (SampleScript2 includes the code to run DataPreprocessing.r)
