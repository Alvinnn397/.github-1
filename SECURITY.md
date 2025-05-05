Please use https://g.co/vulnz to report security vulnerabilities.

We use https://g.co/vulnz for our intake and triage. For valid issues we will do coordination and disclosure here on
GitHub (including using a GitHub Security Advisory when necessary).

The Google Security Team will process your report within a day, and respond within a week (although it will depend on the severity of your report).
https://developers.googleblog.com/en/agent-development-kit-easy-to-build-multi-agent-applications/?utm_source=email&utm_medium=newsletter&utm_campaign=core_aprilhttps://developers.googleblog.com/en/agent-development-kit-easy-to-build-multi-agent-applications/?utm_source=email&utm_medium=newsletter&utm_campaign=core_april
from google.adk.agents import LlmAgent 
from google.adk.tools import google_Search

dice_agent = LlmAgent(
    model="gemini-2.0-flash-exp", # Required: Specify the LLM 
    name="question_answer_agent", # Requdired: Unique agent name
    description="A helpful assistant agent that can answer questions.",
    instruction="""Respond to the query using google search""",
    tools=[google_search], # Provide an instance of the tool
)

# you can run this by using adk web
yussoncariss
