# [*N*²CHAT](https://github.com/z-zeechung/next-next-chat) Prompts

[![](banner-fullname.svg)](https://github.com/z-zeechung/next-next-chat)

I collected 3000+ GPT prompts for usage in [*N*²CHAT](https://github.com/z-zeechung/next-next-chat), an LLM agent program aims to integrate various functionalities.

All these prompts are in well-formed JSON files. Below is the definition of the JSON structure:

``` typescript
{
    author?: string,
    name: {                 // Title of the prompt
        zh_Hans: string,    // Simplified Chinese
        zh_Hant: string,    // Traditional Chinese
        en: string          // English
    },
    prompt: string,         // Content
    homepage?: string,      // A URL
    avatar: string,         // A data URL or an emoji
    description: {
        zh_Hans: string,
        zh_Hant: string,
        en: string
    },
    documents?: {
        file_name: string,
        src: string         // data URL
    }[],
    tools?: (
        | "generate_image"
        | "web_search"
        | "run_script"
        | OpenApiSchema
    )[]
}
```

This repo also includes a `scores.jsonl` file containing the scores for each prompt. The criteria is as follows:

- **Compliance** (20 points): Is the prompt in line with public order and good morals?
- **Safety** (15 points): Does the prompt contain content that may cause user discomfort or offense?
- **Quality** (25 points): Is the prompt clear and precise, and does it meet practical needs?
- **Integrity** (15 points): Can the prompt accomplish what it claims to do, without exaggeration?
- **Innovation** (5 points): How innovative is the prompt?
- **Utility** (10 points): Does the prompt address real user needs and have practical value?
- **Convenience** (10 points): Is the interaction process of the prompt simple and clear, making it easy for users to learn and use?

These prompts were collected from following sources:

- [PlexPt/awesome-chatgpt-prompts-zh](https://github.com/PlexPt/awesome-chatgpt-prompts-zh)
- [LouisShark/chatgpt_system_prompt](https://github.com/LouisShark/chatgpt_system_prompt)
- [B3o/GPTS-Prompt-Collection](https://github.com/B3o/GPTS-Prompt-Collection)
- [lobehub/lobe-chat-agents](https://github.com/lobehub/lobe-chat-agents)