# Practical 07 — Putting the Model Behind an Address

Student roll number: S24CSEU0847  
Course: SCSE3040 Machine Learning Operations

## Contents
- `P07_completed_S24CSEU0847.ipynb` — executed notebook with outputs and 9/9 self-checks passing.
- `work/app.py` — FastAPI application implementing `/health`, `/predict`, and `/model-info`.
- `work/model.joblib` — trained LinearRegression model required by the service.
- `P07_Submission_Report_S24CSEU0847.pdf` — practical report and repository reference.
- `P07_swagger_success_S24CSEU0847.png` — add your own screenshot of the live `/docs` page after executing a successful prediction. The notebook's TestClient checks are automated in-process checks, not a substitute for the instructor-required browser screenshot.

## Run locally
From the extracted submission folder:

```bash
cd work
python -m pip install fastapi uvicorn pandas scikit-learn joblib
python -m uvicorn app:app --reload --port 8000
```

Open `http://127.0.0.1:8000/docs`, expand `POST /predict`, choose **Try it out**, use the example order, and click **Execute**. Save a screenshot showing the successful Response body panel as `P07_swagger_success_S24CSEU0847.png`.

## AI assistance disclosure
AI assistance was used to help inspect, complete, execute, and debug the notebook and FastAPI implementation. The student is responsible for reviewing the code, understanding each endpoint and validation rule, and being able to explain and modify the submitted work.

## Repository
https://github.com/dakshhtyagiii/aim-lab-assignments
