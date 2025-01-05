# Step 2: Setting Up Your Next.js Project

Now that you have GitHub Copilot installed, let's create a Next.js project that we'll use throughout this course.

## Tasks
1. Initialize a new Next.js project:
   ```bash
   npx create-next-app@latest demo-app --typescript --tailwind --eslint
   ```

2. Project Configuration:
   - Choose TypeScript: Yes
   - Choose Tailwind CSS: Yes
   - Choose App Router: Yes
   - Choose custom import alias: Yes (@/*)

3. Create the following structure:
   ```
   demo-app/
   ├── src/
   │   ├── app/
   │   │   └── page.tsx
   │   ├── components/
   │   │   ├── Header.tsx
   │   │   └── Footer.tsx
   │   └── styles/
   └── .github/
       └── copilot/
   ```

## Using Copilot
Try these prompts with Copilot:
- Type `/// Create a responsive header component with logo and navigation`
- Type `/// Create a footer component with social links`

## Validation
To complete this step:
1. Push your Next.js project to your repository
2. Comment "Next.js setup complete"

## Tips
- Use descriptive comments to get better suggestions from Copilot
- Try using Copilot to generate component boilerplate
- Experiment with different comment styles to see how they affect suggestions
