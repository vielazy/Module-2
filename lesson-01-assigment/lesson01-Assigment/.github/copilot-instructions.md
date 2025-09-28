# Copilot Instructions for AI Agents

## Project Overview
This is a simple Java project structured for educational purposes. It consists of two main source files in the `src/` directory: `App.java` (entry point) and `Systemtime.java` (utility or secondary class). The project is designed to be built and run in Visual Studio Code using the Java extension pack.

## Folder Structure
- `src/`: Java source files
- `bin/`: Compiled `.class` files (output)
- `lib/`: Place for external JAR dependencies (currently empty)
- `.vscode/settings.json`: Customizes source/output paths and library references

## Build & Run Workflow
- **Build:** Use the VS Code task labeled `build` or run `msbuild /property:GenerateFullPaths=true /t:build /consoleloggerparameters:NoSummary` in the workspace root.
- **Run:** Execute the main class (`App`) using the Java extension's run/debug features or via command line: `java -cp bin App`.
- **Dependencies:** Place any required JARs in `lib/` and they will be referenced automatically.

## Key Conventions
- All source files must be placed in `src/`.
- Output is always generated in `bin/`.
- External libraries must be JARs in `lib/` and referenced in `.vscode/settings.json`.
- No package declarations are used; all classes are in the default package.

## Patterns & Examples
- Main entry point: `App.java` with a standard `public static void main(String[] args)` method.
- Utility classes (e.g., `Systemtime.java`) should follow similar structure, but may have custom methods.
- Example minimal main class:
  ```java
  public class App {
      public static void main(String[] args) {
          System.out.println("Hello, World!");
      }
  }
  ```

## Integration Points
- No external services or APIs are integrated.
- No test framework is present; add tests in `src/` if needed and update build/run instructions accordingly.

## Tips for AI Agents
- Always update `.vscode/settings.json` if changing source/output/library paths.
- Reference `README.md` for basic project setup and workflow.
- Keep code in the default package unless refactoring for larger scale.
- If adding dependencies, ensure JARs are placed in `lib/` and referenced in settings.

---
If any conventions or workflows are unclear, please ask for clarification or provide suggestions for improvement.
