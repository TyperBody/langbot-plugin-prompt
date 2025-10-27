# Helloprompt

This plugin provides a template for prompt plugin distribution. You can modify the `content` in the following code snippet located at `HelloPrompt/components/event_listener/prompt.py` to implement your prompt writing:

```python
prompt = message.Message(
    role="system",
    content=f'You are a helpful assistant.',
)
event_context.event.default_prompt.append(prompt)
prompt = message.Message(
    role="system",
    content=f'This is a test.',
)
event_context.event.default_prompt.append(prompt)
```

Through this example, you can even implement more complex logic. 