# Screenshots pending refresh

Window: `v2026.609.0` → parent `master` HEAD (`1b89a8e`), nightly run 2026-06-17. (No UI sources changed since the prior run — the only new upstream commit was a Dockerfile fix; the stale set below is unchanged.)

Stale entries are those whose `depends_on` UI source changed within this cumulative window. 62 of 276 registry entries are affected.

Refresh with `npm run screenshots:refresh` (captures stale entries into a review PR — never auto-pushed).

## Stale by changed UI source

- `ui/src/components/AgentConfigForm.tsx` → agent-config captures (20 entries, light + dark)
- `ui/src/pages/CompanySkills.tsx` → company skills captures (12 entries) — note the Skills Store foundation work is in flight; the discovery/detail surfaces are still storybook-only and not yet shipped as pages.
- `ui/src/pages/IssueDetail.tsx` → issue detail/chat/activity/sidebar captures (10 entries)
- `ui/src/pages/RoutineDetail.tsx` → routine detail / cron picker / run-history (6 entries)
- `ui/src/pages/NewAgent.tsx` → new-agent flow (4 entries)
- `ui/src/components/OnboardingWizard.tsx` → onboarding wizard (4 entries) — onboarding is mid-redesign (NUX variants / `OnboardingChat`, A/B-gated); capture after the variant settles.
- `ui/src/components/SidebarCompanyMenu.tsx` → sidebar company menu (4 entries)
- `ui/src/pages/Routines.tsx` → routines list (2 entries)
- `ui/src/pages/InstanceExperimentalSettings.tsx` → experimental settings (2 entries) — now hosts the Conference Room Chat toggle (experimental, flag-gated).

> Note: several of these UI surfaces changed as part of experimental / feature-flagged work (dark-mode theming, onboarding NUX variants, Conference Room Chat). Hold recaptures of the experimental surfaces until the flags settle so the live docs don't show transient states.
