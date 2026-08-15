# CEUSReport

CEUSReport is a desktop application for analysing and reporting contrast-enhanced ultrasound (CEUS) examinations.

Workflow: DICOM import -> cine preprocessing -> ROI selection -> time–intensity analysis -> parametric mapping -> quantitative assessment -> report generation.

# Technical information
Built with Python 3.11+ and PySide6. Supports multiframe ultrasound DICOM, B-mode and contrast-mode views, image stabilization, multiple ROIs, time–intensity curves, model fitting, CEUS perfusion metrics, parametric maps, and distribution statistics.

Export formats: PDF, DOCX, JSON, CSV, image packages, DICOM Structured Reports (DICOM-SR).

# Features
- Multi-ROI CEUS analysis and comparison
- Image stabilization and ROI selection
- Time–intensity curve analysis and model fitting
- CEUS perfusion metrics
- Parametric maps and ROI-based distribution analysis
- Full, clinical-core, and summary report profiles
- Report preview and configurable report content
- Export-time de-identification options
- Processing, quality, provenance, and metric-status information
- Cross-platform resource and user-configuration handling

A shared examination/ROI data model keeps measurements, settings, and provenance consistent across export formats.

Raw analysis results are stored separately from report values. Quality problems, missing measurements, and limitations are reported explicitly; they are not silently replaced or presented as valid.

> Important: CEUSReport is under active development and validation. Quantitative results should be interpreted with acquisition conditions, ROI placement, fitting quality, processing history, and clinical context. 
DICOM metadata de-identification does not guarantee removal of identifying information embedded in image pixels.
