# Fix WPilot Server Port Conflict for Deployment (EADDRINUSE on PORT=10000)

## Steps:
- [x] 1. Update wpilots.js: Differentiate HTTP (use $PORT) and WS ports (ws_port=6114).
- [x] 2. Test locally: `node wpilots.js` - HTTP on 8000, WS on 6114. ✅ Server running without EADDRINUSE.
- [ ] 3. Kill test processes if needed: `npx kill-port 8000 6114 10000`.
- [ ] 4. Set env for test: `set PORT=10000 && node wpilots.js` - HTTP 10000, WS 6114.
- [ ] 5. Verify client connects to ws://localhost:6114/.
- [ ] 6. Deploy to Render; set WS_PORT env if needed (default 6114 often open).
- [ ] 7. Mark complete.

Progress: Starting edits...
