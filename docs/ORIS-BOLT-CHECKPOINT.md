# Bolt.new independent specialist — checkpoint (2026-10-15)

## Purpose
Keep this fork as a standalone rapid application-building specialist that ORIS can invoke later. Do NOT merge into the existing ORIS Workshop (based on bolt.diy). Preserve the original behavior initially; rebrand only after testing.

## Verified during guided Codespaces session
- Fork: EzenielEmmanuel/bolt.new from stackblitz/bolt.new, main branch.
- StackBlitz WebContainer: Cloudflare workerd executable error; app did not launch there.
- GitHub Codespaces (ideal-space-yodel): Node v24.21.0; pnpm v9.4.0.
- pnpm install completed; pnpm run dev started Remix/Vite on port 5173.
- Private forwarded preview displayed the Bolt.new home interface.
- Attempted AI prompt returned a processing error.
- Terminal included vercel.ai.error.AI_LoadAPIKeyError.
- Source reference app/lib/.server/llm/api-key.ts:8 resolves env.ANTHROPIC_API_KEY || cloudflareEnv.ANTHROPIC_API_KEY.
- AI coding performance and model availability NOT yet verified.

## Resume plan
1. Resume Codespace or use an appropriate Linux environment; run pnpm run dev if necessary, keep port 5173 private.
2. Inspect required Anthropic configuration and use Codespaces secrets / secure environment configuration; never commit or share API keys.
3. Verify actual model access and conduct small benchmark tasks (startup, first response, task completion, code quality, resource usage).
4. Create a separate rebranding/development branch; preserve licensing, attribution, and upstream tracking.
5. Rebrand the independent Bolt.new specialist; commit a tested stable baseline.
6. Add alternative models, adapters, memory or other intelligence only as justified by demonstrated needs.

## Operational notes
- Codespaces can consume usage allowance while running; stop unused Codespaces.
- Avoid mixing npm and pnpm lockfiles. An automatic Codespaces setup created package-lock.json; it was removed locally before pnpm install.
- This checkpoint documents observed progress; it does not save uncommitted Codespaces workspace files or credentials.
