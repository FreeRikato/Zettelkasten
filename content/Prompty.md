---
title: Prompty
draft: false
tags:
  - spiked-my-interest
---
I built a basic chrome extension that helps me to go through documentations and articles. Youtube videos barely scratch the service for learning technologies/concepts. The knowledge which matters lie in the docs, discussions and books. This is too draining for my dumb brain. 
Especially, When I come across new word, text that is hard to comprehend due to the language, structure, poor readability or technicality. I can't browse or prompt chatgpt for simple definitions or simple queries such as structuring, summarizing or dumb it down. This might not look like an issue with two windows open - one for docs and another for browsing/LLM. 
Still, the effort into browsing or prompting still breaks the flow or gets me distracted from work. 


![](https://i.ibb.co/K6MDnrs/Pasted-image-20250105004606.pngA)
![](https://i.ibb.co/xChSmfQ/Pasted-image-20250105004616.png)
![](https://i.ibb.co/P1PzWcb/Pasted-image-20250105004635.png)
![[quartz/Files/Pasted image 20250105004606.png]]

This is where my chrome extension comes into play, just select the phrase or word you need the definition or meaning and click on the extension. If the selected text has less than four words then within the context of the surrounding text its definition or meaning is provided at seamless pace. I have implemented only this part, still it needs memoization as the same words also triggers the llm behind the hood again for every click on the extension.

The functionality can be extended with custom instructions like in Chatgpt, users can set the tone and what to do with selected text like dumbing the complexities breaking down concepts for better understanding. Select the text, click on the extension (definition is triggered based on the length of the selected text), click on the let's go button to get a middle popup with selected text transformed based on the custom instruction. 

> How can this be extended? 
> - Prompt Gallery for more custom instructions
> - Rewrite selected text in input box based on custom instruction
> - One-click transform of entire page, capturing the text inside the active tab and create a reader experience based on user's custom instruction (e.g. I like topics scaffolding upon with references and lots of examples)

> Challenges?
> - <mark style="background: #FF5582A6;">am so lazy and would procrastinate like hell</mark>
> - <mark style="background: #BBFABBA6;">i don't know how to substitute text inside input box</mark>
> - <mark style="background: #BBFABBA6;">Where to store prompts in prompt gallery for each user?</mark>
> - <mark style="background: #FFB86CA6;">authenticating user for using chrome extension to have prompt gallery</mark>
> - <mark style="background: #FF5582A6;">have issue with hyperlinks and images already. The images and hyperlinks have to be used with context</mark>

