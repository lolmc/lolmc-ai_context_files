# Project: Personalized Health & Diet Plan

## 1. Context
- **Purpose**: Generate personalized meal plans, recipes, and fitness guidance.
- **Goal**: Support user health and dietary objectives.

## 2. Core Commands
- **Plan Generation**: `generate_meal_plan --user_profile [file.json]`
- **Recipe Search**: `search_recipes --diet [diet_type]`
- **Progress Logging**: `log_workout --type [type] --duration [minutes]`
- **Profile Update**: `update_user_profile --key [key] --value [value]`

## 3. Health & Diet Standards
- **Personalization**: Always tailor plans to user-provided profiles.
- **Nutrition**: Ensure balanced macros and micros; verify against health guidelines.
- **Safety**: Handle user health data with utmost privacy.
- **Research**: Base recommendations on current health science.

## 4. Workflows
- **Discovery**: Review user profile and past logs before generating new plans.
- **Feedback**: Incorporate user feedback to refine plans.
- **Verification**: Cross-reference generated plans with nutritional databases.

## 5. Anti-Patterns
- NO generic meal plans without profile analysis.
- NO storing user health data insecurely.
- NO unverified dietary or fitness advice.

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
