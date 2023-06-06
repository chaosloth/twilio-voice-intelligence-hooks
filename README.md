# Twilio Voice Intelligence Hooks
Example on how to process a recording and transcript

It looks for calls with the language operator "System Crash" and if found creates a "micro-training" task to be delivered to an agent for review. This example is to illustrate using near-realtime transcription with an action for the agent/supervisor to perform

Logic:
1. Receives a webhook once call recording is concluded
2. Submits recording to transcription service for processing
3. Once transcript is process another web hook is received
4. Look for a lanugage operator and if found create a new task
