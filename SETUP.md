# Setup Guide

**Getting started with AI-assisted design QA — no technical background required.**

This guide assumes you've never used an AI tool for design work before. If you're already comfortable with ChatGPT or Claude, skip to [Step 3](#step-3-run-your-first-qa-session).

---

## What you'll need

- A free [ChatGPT account](https://chat.openai.com) **or** a free [Claude account](https://claude.ai)
- The project you want to QA (copy doc, design file, exported PDF, or screenshots)
- About 10–15 minutes for your first session

That's it. No plugins, no integrations, no technical setup.

---

## Step 1: Pick your AI tool

Both work. Here's the short version:

| | ChatGPT | Claude |
|--|---------|--------|
| Free tier | Yes | Yes |
| Good at copy/grammar | ✅ | ✅ |
| Good at following long checklists | ✅ | ✅✅ |
| Can analyze images | Yes (GPT-4o) | Yes (Claude 3+) |
| Best for | General use | Long documents, nuanced copy |

**Recommendation:** Start with whichever you already have. They're both good enough.

---

## Step 2: Understand how to use the prompts

The `/prompts` folder contains pre-written instructions you paste into the AI chat. Think of them as a briefing you give an assistant before handing off a task.

**How it works:**
1. Open the prompt file (e.g., `prompts/copy-review-prompt.md`)
2. Copy the entire prompt
3. Paste it into a new ChatGPT or Claude conversation
4. Then paste your copy (or upload your file/screenshot) in the same message
5. Send it and read the response

The AI will work through the checklist items systematically and flag anything that needs attention.

---

## Step 3: Run your first QA session

**For copy review:**

1. Open `prompts/copy-review-prompt.md`
2. Copy the prompt
3. Open a new conversation in ChatGPT or Claude
4. Paste the prompt, then on a new line paste your copy document
5. Hit send

**For design review:**

Design QA is partially visual, so you'll need to either:
- Export a PDF and upload it, or
- Take screenshots of your key screens/pages and upload them

The AI can review text content directly from files, and can assess visual layouts from screenshots.

---

## Step 4: Use the checklists alongside the AI

The checklists in `/checklists` are your reference layer — the things to check *even when* the AI has reviewed the work.

Items marked **👁️ Needs human judgment** are things the AI will flag but can't fully evaluate. You make the call on those.

**Workflow suggestion:**
1. Run the AI prompt first → get a pass on all the mechanical stuff
2. Review the AI's output
3. Walk through the checklist manually for the human-judgment items
4. Fix anything flagged
5. Run final handoff checklist before delivery

---

## Step 5: Build it into your process

The system works best when it's not an afterthought. Two places to slot it in:

**Before creative review:** Run copy QA before you send work to a creative director or for internal review. Catch errors before they become comments.

**Before client delivery:** Run the full handoff checklist before anything goes out the door. Every time.

---

## Tips from actual use

- **Be specific with AI.** If you tell it "check this copy," it gives you a generic response. If you paste the full prompt first, it follows the checklist systematically.

- **AI can't read brand guidelines it doesn't have.** If brand consistency is critical, paste relevant sections of the brand guide into the same conversation before asking for a review.

- **Screenshots work better than you'd expect.** Upload a screenshot of your design and ask the AI to check for widows, orphans, and line breaks — it can often catch these visually.

- **Start a new conversation for each project.** AI tools have memory limits. A fresh conversation for each QA session keeps things clean.

---

## Troubleshooting

**"The AI didn't follow the checklist structure."**
Make sure you're pasting the full prompt before your content, not after. The prompt primes the AI on what to do.

**"The AI missed obvious errors."**
Try being more explicit: after pasting the prompt, add "Please be thorough and flag every instance, even minor ones."

**"The AI gave me a wall of text that's hard to parse."**
Add to the end of your prompt: "Format your response as a numbered list with the checklist item, your finding, and a suggested fix."

---

*Questions or issues? Open a GitHub issue.*
