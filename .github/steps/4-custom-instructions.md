# Step 4: Implementing Custom Instructions

Now let's create custom instructions for GitHub Copilot to better understand your project's requirements and coding standards.

## Tasks

1. Create Custom Instructions File
   Create `.github/copilot/custom-instructions.md` with the following sections:

   ```markdown
   # GitHub Copilot Custom Instructions

   ## Project Context
   This is a Next.js 14 project using:
   - TypeScript for type safety
   - Tailwind CSS for styling
   - ESLint for code quality
   - React Server Components
   
   ## Coding Standards
   - Use functional components with TypeScript
   - Implement proper prop types and interfaces
   - Follow React hooks best practices
   - Use meaningful variable and function names
   - Include JSDoc comments for complex functions
   
   ## File Organization
   - Components go in `src/components`
   - Pages go in `src/app`
   - Types go in `src/types`
   - Utils go in `src/utils`
   
   ## Component Structure
   - One component per file
   - Export as named exports
   - Include prop interface above component
   - Add component documentation
   
   ## Testing Requirements
   - Write unit tests for utilities
   - Create component tests with React Testing Library
   - Follow Testing Library best practices
   ```

2. Test Custom Instructions
   - Create a new component using Copilot
   - Verify it follows your custom instructions
   - Make adjustments as needed

## Validation
1. Push your custom instructions file
2. Create a test component using the instructions
3. Comment "Custom instructions implemented"

## Tips
- Be specific about coding patterns
- Include examples in your instructions
- Update instructions as your needs change
- Test instructions with different components
