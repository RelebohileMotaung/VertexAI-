# LLM powered Chatbox using VertexAI

```
conda create -n chatbot python=3.10 -y
```
```
conda activate chatbot
```
```
pip install -r requirements.txt
```

```
gcloud builds submit --tag gcr.io/YOUR-PROJECT-ID/gemini-flask-app
```

### Deploy to Cloud Run
```bash
gcloud run deploy gemini-flask-app \
  --image gcr.io/YOUR-PROJECT-ID/gemini-flask-app \
  --platform managed \
  --region us-central1 \
  --allow-unauthenticated \
  --set-env-vars "project_id=YOUR_PROJECT_ID" \
  --set-env-vars "region=YOUR_REGION" \
  --memory 1Gi \
  --cpu 2
```