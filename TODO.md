# WPilots Server Fix Plan
Track progress on fixing the broken server code in wpilots.js.

## Steps:
- [x] 1. Create this TODO.md
- [ ] 2. Fix malformed requires in wpilots.js (add newlines, fix indentation, remove stray \\n)
- [ ] 3. Modernize WebSocketServer creation (uncomment, add 'new', use options.port/host)
- [ ] 4. Define PORT/options before use in start_gameserver
- [ ] 5. Fix minor issues in lib/fu.js (var process shadowing)
- [ ] 6. Add missing utilities (get_time, round_number)
- [ ] 7. Test: npm install & node wpilots.js
- [ ] 8. Verify HTTP/WS servers start, serve client/index.html

Next step: Fix requires via edit_file on wpilots.js.

