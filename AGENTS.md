# Agent Instructions for Parcourssup (Symfony PHP Project)

## Project Commands
- Run development environment: `npm run dev`
- Create new Symfony component: `npm run new [name]`
- Run Symfony command: `npm run symfony [command]`
- Run Composer command: `npm run composer [command]`
- Start Symfony server: `npm run serve`
- Run tests: `npm run symfony php bin/phpunit`
- Run single test: `npm run symfony php bin/phpunit tests/path/to/TestFile.php`
- Run PHP CS Fixer: `npm run composer run-script cs-fix`
- Run PHP Stan: `npm run composer run-script analyse`

## Code Style Guidelines
- Follow PSR-12 coding standards for PHP
- Use strict typing with PHP 8.2 features
- Use meaningful namespaces following Symfony conventions
- Class names: PascalCase (MyClass)
- Method names: camelCase (myMethod)
- Variables/properties: camelCase (myVariable)
- Constants: UPPER_SNAKE_CASE (MY_CONSTANT)
- Prefer constructor property promotion
- Use type hints for parameters and return types
- Handle exceptions with appropriate try/catch blocks
- Use dependency injection following Symfony best practices
- Document public APIs with PHPDoc comments
- Keep methods small and focused on a single responsibility