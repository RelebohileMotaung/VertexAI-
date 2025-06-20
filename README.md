# LLM powered Chatbox using VertexAI

conda create -n chatbot python=3.8 -y


conda activate chatbot


pip install -r requirements.txt

gcloud builds submit --tag gcr.io/PROJECT-ID/Name  --project=PROJECT-ID