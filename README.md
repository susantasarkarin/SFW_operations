# Survey Traffic Manager (Backend)

FastAPI skeleton for intelligent survey traffic routing.

Quickstart (Windows PowerShell):
1) Create venv: python -m venv .venv
2) Activate: .venv\Scripts\Activate.ps1
3) Install deps: pip install -r requirements.txt
4) Run: uvicorn app.main:app --reload --host 0.0.0.0 --port 8000

Endpoints:
- Health: GET /health/live, /health/ready
- Intake: GET /take?rId=<PID>-<VID>-<VendorRID>
- Webhooks: GET /surveycomplete?rId=<SID>, /surveyterminate?rId=<SID>, /quotafull?rId=<SID>

Next Steps:
- Add SQL and Mongo connectors
- Implement session creation, fraud stubs, idempotent webhooks
- Add structured logging, config, and tests
