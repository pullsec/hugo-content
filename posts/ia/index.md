---
title: "How AI Changed the Way I Learn Cybersecurity"
date: 2026-05-02T10:43:23+02:00
lastmod: 2026-05-02T16:02:43+02:00
comment: false
type: posts
toc:
  enable: true
tags:
  - journey
categories:
  - thought
expirationReminder:
  enable: false
featuredImagePreview: "/images/covers/ia.png"
---

I’ve been learning cybersecurity through labs, writeups, and by building my own environment.
At the beginning, like most people, I relied a lot on Google and StackOverflow.  

<!--more-->

Whenever something didn’t work, I would search for the error, open multiple tabs, and try to find something that looked close enough to my situation.

It worked… sometimes. But over the past few months, I noticed something interesting. I almost stopped using StackOverflow. Not because it became irrelevant, but because my way of approaching problems changed.


## Before vs Now

Before, when I encountered an issue, my process was quite mechanical. I would search for the exact error message, browse through different threads, and try to match someone else’s situation to mine. Most of the time, the answers were either too generic or slightly different from what I needed, which forced me to adapt them blindly.

Today, things feel very different.

Instead of searching for a solution, I start by describing the problem. I include context, what I expected to happen, what actually happened, and any detail that might matter. From there, I iterate. I refine the problem, challenge the answers, and move step by step.

It feels less like searching, and more like exploring.

```mermaid
flowchart LR
    A["Problem"]
        --> B["Search"]
        --> C["Try fix"]

    D["Problem"]
        --> E["Describe"]
        --> F["Iterate with AI"]
        --> G["Understand"]
```

## What AI Actually Changed

The biggest change is not speed. It’s interaction.

With StackOverflow, everything is static. You read what already exists and try to make it fit your situation. With AI, the process becomes dynamic. You can adjust your input, clarify your thinking, and progressively narrow down the problem. Instead of adapting yourself to the answer, you adapt the answer to your context. 

The shift is not just personal — it’s visible at a larger scale.

```echarts
{
  "title": {
    "text": "Shift in Developer Workflow",
    "subtext": "From static answers to interactive debugging",
    "left": "center"
  },
  "tooltip": {
    "trigger": "axis"
  },
  "legend": {
    "top": "12%",
    "data": [
      "StackOverflow-style search",
      "AI-assisted debugging"
    ]
  },
  "grid": {
    "left": "5%",
    "right": "5%",
    "bottom": "8%",
    "top": "26%",
    "containLabel": true
  },
  "xAxis": {
    "type": "category",
    "boundaryGap": false,
    "data": [
      "2018",
      "2019",
      "2020",
      "2021",
      "2022",
      "2023",
      "2024",
      "2025",
      "2026"
    ]
  },
  "yAxis": {
    "type": "value",
    "min": 0,
    "max": 100,
    "axisLabel": {
      "formatter": "{value}%"
    }
  },
  "series": [
    {
      "name": "StackOverflow-style search",
      "type": "line",
      "smooth": true,
      "symbol": "circle",
      "symbolSize": 7,
      "lineStyle": {
        "width": 3
      },
      "areaStyle": {
        "opacity": 0.12
      },
      "data": [
        100,
        98,
        96,
        94,
        85,
        65,
        48,
        30,
        20
      ],
      "markLine": {
        "symbol": "none",
        "lineStyle": {
          "type": "dashed"
        },
        "data": [
          {
            "xAxis": "2022",
            "label": {
              "formatter": "ChatGPT released"
            }
          }
        ]
      }
    },
    {
      "name": "AI-assisted debugging",
      "type": "line",
      "smooth": true,
      "symbol": "circle",
      "symbolSize": 7,
      "lineStyle": {
        "width": 3
      },
      "areaStyle": {
        "opacity": 0.12
      },
      "data": [
        2,
        3,
        5,
        8,
        25,
        55,
        72,
        88,
        95
      ]
    }
  ]
}
```

> trend: static answers ↓ | interactive debugging ↑

This is not exact data, but it reflects a trend that is becoming hard to ignore. Public traffic data also shows that StackOverflow usage started to decline shortly after the release of ChatGPT in late 2022, reinforcing this shift.

## A Concrete Example

At some point, while working on a small lab, I had a binary that kept crashing. I tried the usual approach first, checking documentation and searching online, but nothing really matched what I was experiencing.

So I changed approach.

I started explaining the situation more clearly, including what I had already tried and what I expected to happen. From there, I began iterating. Each step gave me a slightly better understanding of what was going on.

Was the AI always correct? Not at all.

But it helped me move forward. It suggested directions, sometimes wrong ones, but enough to keep me thinking and testing instead of being stuck.


## The Limits

It’s important to be clear about this. AI is not a replacement for understanding. It can be wrong, sometimes confidently wrong. It can oversimplify problems, or miss important technical details, especially in more advanced cybersecurity scenarios.

If you rely on it blindly, you will eventually hit a wall.
In fact, the more technical the problem gets, the more you need your own reasoning to guide the process.

> [!WARNING]
> AI can confidently give wrong answers.  
> In cybersecurity, blindly trusting it can lead to incorrect reasoning or completely broken approaches.

## What I Learned

The main thing I realized is that AI doesn’t replace knowledge, it amplifies it. If you already have a way of thinking, even a basic one, it helps you move faster. It allows you to test ideas quickly, to explore different paths, and to stay engaged with the problem.

But if you don’t understand what you’re doing, it doesn’t magically solve that.

You still need to think.

## Final

I don’t think AI replaces StackOverflow. But it clearly changes how I learn and how I approach problems. Instead of searching for answers, I spend more time trying to understand the problem itself. And in cybersecurity, that difference matters a lot.

Understanding will always be more valuable than memorizing solutions.
And in that sense, AI is not replacing learning it’s just changing the way we get there.
