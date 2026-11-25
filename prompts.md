# Prompt templates for Gemma models

Starting templates only; they are not tested outputs or benchmark prompts. Replace bracketed text and use only fields supported by the chosen route.

## Character brief

```text
Use this character brief consistently. Write a short scene that reveals personality through choices and dialogue: [brief].
```

## Image description

```text
Describe the composition and mood of this image. Separate visible details from interpretation: [image].
```

## Draft revision

```text
Revise this passage for clarity and rhythm while preserving its meaning and point of view: [passage].
```

## Image prompts

For a route that accepts image_url, provide the image as a separate request field and refer to it in prompt. Do not assume a text-only route can fetch or inspect an image URL.
