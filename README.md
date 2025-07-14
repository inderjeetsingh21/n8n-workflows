# n8n-workflows

## Content Writer
 - The workflow uses the concept called Parallel Expert Synthesis
 - The worflow starts with a webhook, and then the fields can be parsed through the Edit block into the AI Agents
 - The begining fields are Topic, Platform and Tone. 
 - Sample webhook JSON request looks like this

<code>
    {
    "sessionId": "session_md3ev8l3_x09q3ii3d",
    "Topic": "create 3 ideas on DIY Pottery",
    "Platform": "LinkedIn",
    "Tone": "inspirational"
    }
</code>

 - The workflow has the following flow

        ┌────────────────────┐
        │Form or Webhooks    │
        └────────┬───────────┘
                 ▼
            ┌────────────┐
            │  Intent    │
            └────┬───────┬────────┬────────┐
                 ▼       ▼        ▼        ▼
            Reasoning  Emotion  Outline  Final Post




