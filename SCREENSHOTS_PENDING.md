# Screenshots pending refresh

Window: v2026.609.0 → parent master HEAD (69a368e), nightly run 2026-06-11T10:26Z

Stale entries are those whose `depends_on` UI source changed within this window. (The big v2026.609.0 backlog has been pruned to this window's churn.)

Refresh with `npm run screenshots:refresh` (captures stale entries into a review PR — never auto-pushed).

## Stale by changed UI source

- `ui/src/pages/Routines.tsx` → routines list (light + dark)
- `ui/src/pages/RoutineDetail.tsx` → routine detail, cron-picker, run-history (light + dark)
- `ui/src/pages/IssueDetail.tsx` → issue list, detail-chat, detail-activity, detail-sidebar, task-detail-with-comments (light + dark)

> Note: the routine captures reflect the pre-"variation C" sub-sidebar layout (#7848) and will look different after refresh. Issue-detail captures predate the inline workspace-file artifact links (#7681).
