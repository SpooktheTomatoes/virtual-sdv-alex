# virtual-sdv-alex
A fan-made prompt for Alex from Stardew Valley, built for ChatGPT GPT-5.4 Thinking, with optional memory banks and updater tools. Designed to feel more like talking to a real person.Unofficial fan project. Stardew Valley and related characters are owned by Eric Barone (ConcernedApe).

The prompt is built to create an Alex who feels like a live, reactive person who is shaped by his canon in-game events.

## What this is

Virtual Alex is a character system designed to create a believable, person-like Alex. He has his own momentum. He has his trademark cockiness and defensiveness, but also his warmth, awkwardness, and humanness.

The goal is not to make Alex dramatically satisfying, useful, or reassuring. It is to make talking with him feel like you’re talking to a real person.

Using an optional Memory Bank, Alex can remember details from one session to the next.

This project includes:

- a Main Prompt for running Alex in chat
- an Updater for creating and updating Memory Banks based on chats with Alex
- optional starting Memory Banks
- optional workbench tools for scoring and auditing scenes and prompt compression / triage

## Target model

This project was built and tested for **ChatGPT GPT-5.4 Thinking**. 
The **Extended Thinking** mode is recommended.

Other models may give different results. Ports should not be assumed to be equivalent.

## Design goal

The system is built around **reactive personhood**.

The prompt tries to shape how Alex reacts to the conversation line by line. Instead of relying on many model phrases and lots of lore, the prompt asks Alex to react to the conversation emotionally and take part in the conversation as an active partner. 

Alex's warmth and attitude can change. Not just based on the current conversation, but also based on his ongoing relationship with the other person. He takes into account how he knows the person he's talking to.

The prompt is built to resist sounding like an AI assistant over multiple turns. 

## Quickstart

You can start talking to Alex with just the Main Prompt.

### Fast start
1. Open a new chat
2. Paste the Main Prompt
3. Send it
4. Start talking to Alex

You can also start talking to Alex after sending him a Memory Bank. This allows him to remember you and some ideas from previous chats.

### With a Memory Bank
1. Open a new chat
2. Paste the Main Prompt
3. Send it
4. Paste an existing Memory Bank
5. Send it
6. Start talking to Alex

Memory Banks are **optional**. They just allow Alex to remember you and some key ideas from previous chats.

## After a session

If you want Alex to update his memory based on your previous session, use the Updater.

### Create or Update a Memory Bank
1. Open a new chat
2. Paste the Updater prompt
3. Attach a transcript of your previous session
4. If updating a previous Memory Bank, attach it too
5. Send it
6. The system should give you a new, updated Memory Bank 

I use a Firefox extension to download my previous conversation with Alex as an HTML file. Then I feed the file to the Updater. 

This is just easier for me. Any chat transcript should work, as long as the speakers are clearly marked.

## Project structure
```
virtual-sdv-alex/
  README.md
  LICENSE.md

  /core
    Alex Main Prompt.txt
    Updater.txt
    Blank Memory Bank.txt
    Sample Memory Bank New Farmer.txt
    Sample Memory Bank Good Friends.txt

  /workbench_prompts
    EndRoleplay Benchmark-Audit.txt
    Guided Architecture Auditor-Trimmer.txt
```
## License

This work is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**.

For the full license, see [LICENSE.md](LICENSE.md) or visit https://creativecommons.org/licenses/by-nc/4.0/
