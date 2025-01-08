Chromes extensions are useful piece of software that i have been exploring recently. Spending a lot of time in the browsers, the extensions are capable of helping us in a lot of way. I have always felt them magical and wondered how would one build it. 

I tried to build one and came up with [[Prompty|Prompty]], an extension that would help me to quickly see definitions and prompt the underlying large language model to perform a task with selected task. I learned a lot while building it, felt it it to be so easy & cool and will try my best to teach what i have learnt. My way of teaching would be first principles approach scaffolding concepts one upon one along with code snippets and building a project. 

**Note**: The tech stack I use in this article is Vite+React+Typescript. A basic understanding of HTML, CSS and Javascript is enough for you to follow along this article.
## Core concepts
>"A chrome extension is a small software program that enhances & customizes the browsing experience. It can access and modify the browser's UI elements, interact with web pages (via content scripts), and run in the background to provide persistent or on-demand features."

Every chrome extension starts with a `manifest.json` file. This acts as the blueprint for the extension, telling chrome what the extension is, what is does, and what permissions it needs.

```json
// manifest.json: Keep this at the root of the project's src directory or public, as Vite will handle it during the build process
{
  "manifest_version": 3, // Specifies manifest file format version. Use 3 for modern extensions
  "name": "Hello world Extension", // Name of the extension, visible in chrome web store and extension management page
  "version": "1.0", // Version number of the extension
  "description": "A simple extension." // A brief description for the extension
}
```

## Setting up environment
```bash
npm create vite@latest chrome-extension -- --template react-ts
cd chrome-extension
npm install
npm install --save-dev @types/chrome
```

The project file tree would look like,
```text
chrome-extension/
├─ public/
├─ src/
│  ├─ App.tsx
│  ├─ main.tsx
│  └─ vite-env.d.ts
├─ index.html
├─ package.json
├─ tsconfig.json
└─ vite.config.ts
```

Sources:
1. [FreeCodeCamp: Building-chrome-extension](https://www.freecodecamp.org/news/building-chrome-extension/)
2. https://scribehow.com/library/how-to-create-a-chrome-extension
3. https://daily.dev/blog/writing-extensions-for-chrome-a-developers-guide
4. https://www.geeksforgeeks.org/building-basic-chrome-extension/