# travel-reimbursement-approval-agent
AI-assisted Travel Reimbursement Approval Agent using deterministic policy tools, LangChain, Groq integration, audit trails, structured outputs, and dashboard reporting. 

Purpose
The Travel Reimbursement Approval Agent evaluates claims using the supplied travel policy and returns transparent, auditable, and structured recommendations.

Key Capabilities
Accepts reimbursement claims represented as structured Python dictionaries equivalent to JSON input.
Retrieves relevant policy rules by stable POL-* identifiers.
Calls specialized tools for:
Category eligibility
Receipt completeness
Airfare-class compliance
Per-diem and category limits
Submission timeliness
Approval thresholds
Output validation
Preserves an audit trail of the tools and policies used.
Routes missing, conflicting, exceptional, or high-value cases to MANUAL_REVIEW.
Produces a JSON array containing exactly the required output fields.
Generates a dashboard from the actual evaluated claim results.
Runtime Requirements
Python 3.10 or later
Jupyter Notebook
pandas
matplotlib 
ipywidgets

Setup
Create and activate a virtual environment, then install the required packages:

python -m venv .venv
.venv\Scripts\activate
python -m pip install notebook pandas matplotlib ipywidgets
jupyter notebook
