# LLMux, a Large Language Model operating system for general purpose life long learning

**Notice: This project is the predecessor of [NPython](https://github.com/20171130/NPython) and is no longer updated.**

llmux is an operating system on Large Language Models that provides an abstraction layer with basic funtionalities such as multiagent concurrency and communication, long-term memomy management, device management, etc.
It is designed to help building complex applications on large language model chatbots.
llmux is currently an experimental project under rapid development.
We encourage you to build applications and run experiments on llmux.
You can share your user experience, report issues, or start pull requests to help us improve llmux. Your contributions will be greatly appreciated. 
# Install
``` 
pip install -r requirements.txt
```
# QuickStart
You may read the technical note [here](https://drive.google.com/file/d/1hfX_ByGPPdE97I7At4RWmbV0CHO9o7Cx/view?usp=sharing).

First set up the environment variable `OPENAI_API_KEY`. Run `python3 demo.py` for a demo. This script illustrates the basics of llmux. You may read and modify it according to your needs. You can start your message with "! ' to evaluate an expression. Call `! system.exit()` to exit gracefully. You can only see messages sent to you on the terminal. To inspect all messages, such as messages between a bot and the system or messages between bots, inspect the output files. By default the output path is "/home/ubuntu/llmux_output", you can modify this in "demo.py"
# Citations
```
@misc{llmux,
      title={An Operating System on Large Language Models for General-Purpose Lifelong Learning}, 
      author={Hangrui Bi},
      year={2023}
}
```
# ToDo

1. More testing and prompt engineering.
2. Improve the regex used for extracting codes in 'bot.py'.
3. Improve the format error messages, distinguish error types, identify unsuccessful function calls and warn.
4. Implemenet more devices.
5. Add an event handler to write old messages into the long-term memory.
6. Implement advanced memory management, compression and garbage collector.
7. Load balance among multiple backends.
8. Allow event handlers to filter messages within a peer.
9. Support large long-term device that does not fit in RAM.
