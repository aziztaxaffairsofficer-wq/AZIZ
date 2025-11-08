# Veo3 Video Generator (example)

Contoh repo untuk menghasilkan video menggunakan model Veo 3 melalui Google Vertex AI (REST).

## Persiapan
1. Aktifkan Vertex AI API di Google Cloud Console.
2. Buat Service Account dengan role yang diperlukan (Vertex AI Admin / atau role yang lebih terbatas untuk generative models).
3. Download JSON key dan set environment variable:
   export GOOGLE_APPLICATION_CREDENTIALS="/path/to/key.json"
4. Catat: PROJECT_ID dan LOCATION (mis. us-central1).
5. Pastikan model Veo3 tersedia untuk project (akses model via Model Garden / Google AI Console).

## Cara pakai
1. Install dependensi:
   pip install -r requirements.txt

2. Edit `main.py` untuk mengganti `PROJECT_ID`, `LOCATION`, dan `MODEL_ID` (mis. 'veo-3' atau 'veo-3-1').

3. Jalankan:
   python main.py --prompt-file prompts/example_prompt.txt
