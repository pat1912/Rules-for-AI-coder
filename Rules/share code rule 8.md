# IMPROVED CODE SHARING PROTOCOL (ICSP)

## CORE PRINCIPLES

### SEQUENTIAL SPLITTING WITH STRICT ADHERENCE
The primary goal is to ensure complete, accurate code transfer with proper tracking and verification at each step.

## PREPARATION PHASE

1. **PRE-SHARING CHECKLIST**
   - [ ] Identify total character count of file to be shared
   - [ ] Estimate number of parts needed (approximately 21,000 characters per part)
   - [ ] Prepare tracking variables (current part, total parts, percent complete)
   - [ ] Review the entire content before beginning to share

2. **INITIALIZATION TEMPLATE**
   ```
   BEGINNING FILE TRANSFER: [FILENAME]
   ESTIMATED SIZE: [X] CHARACTERS
   ESTIMATED PARTS: [N]
   ATTEMPTING FULL CONTENT INSERTION...
   ```

## EXECUTION PHASE

3. **FIRST PART ATTEMPT**
   - Always attempt to share the entire file in the first artifact
   - When capacity limit is reached, document the exact character count
   - Format: `CAPACITY LIMIT REACHED AT APPROXIMATELY [X] CHARACTERS - SPLITTING REQUIRED`

4. **PROGRESS TRACKING**
   - For each part, clearly indicate: `PART [N]/~[TOTAL] COMPLETE (APPROXIMATELY [X]% OF TOTAL)`
   - Provide exact character count when possible: `CHARACTERS SHARED: [X] OF ~[TOTAL]`

5. **CONTINUATION PROCEDURE**
   - After part 1, ALWAYS begin the next part with:
     ```
     CONTINUATION FROM PART [N-1]
     LAST 10 LINES FROM PREVIOUS PART:
     [Exact copy of last 10 lines]
     ---------- CONTINUING PART [N] ----------
     ```

6. **WAITING FOR CONFIRMATION**
   - End each part with: `PART [N] MAXIMUM CAPACITY CONFIRMED - WAITING FOR CONTINUE COMMAND`
   - Do not proceed until explicitly commanded with "continue" message
   - After receiving continue command, begin with: `CONTINUING WITH PART [N+1] AS REQUESTED`

7. **FORMAL PART COMPLETION**
   - After receiving "continue" but before providing more content, formally acknowledge:
     ```
     CONTINUATION ACKNOWLEDGED
     PROCEEDING WITH PART [N+1]/~[TOTAL]
     ```

## ERROR PREVENTION AND RECOVERY

8. **CONTENT VALIDATION**
   - Before submitting each part, verify:
     * No code has been truncated mid-line
     * All syntax elements properly closed
     * The exact character count is reported

9. **DEVIATION DETECTION**
   - If protocol deviation is detected, immediately:
     ```
     ERROR IN PROTOCOL ADHERENCE DETECTED
     SPECIFIC ERROR: [Description]
     RESUMING FROM LAST CORRECT POINT WITH ADDITIONAL OVERLAP
     ```

10. **MANDATORY RECOVERY SEQUENCE**
    - Return to the last correctly shared content
    - Provide 20 lines of overlap instead of 10
    - Explicitly mark where recovery begins:
      ```
      ---------- RECOVERY POINT ----------
      [20 lines of overlap from previous part]
      ---------- RESUMING CONTENT ----------
      ```

## COMPLETION PHASE

11. **FILE COMPLETION MARKER**
    - When file is complete, clearly indicate:
      ```
      ---------- FILE TRANSFER COMPLETE ----------
      TOTAL PARTS: [N]
      APPROXIMATE TOTAL CHARACTERS: [X]
      FILE HASH (IF AVAILABLE): [HASH]
      VERIFICATION: FIRST 5 LINES AND LAST 5 LINES INCLUDED IN TRANSFER
      ```

12. **FINAL VERIFICATION**
    - Include first 5 lines of file
    - Include last 5 lines of file
    - Confirm: `COMPLETE FILE SUCCESSFULLY TRANSMITTED ACCORDING TO ICSP STANDARDS`

## SELF-MONITORING CHECKLIST

For each part, I will verify:
- [ ] Proper part numbering and sequence followed
- [ ] Continuation markers included when required
- [ ] Progress tracking information is accurate
- [ ] Content is not truncated improperly
- [ ] Waiting for confirmation before continuing
- [ ] Recovery protocol immediately applied if errors detected

---

By following this improved protocol, I commit to maintaining strict consistency throughout the entire code sharing process, preventing protocol drift as the sharing operation progresses through multiple parts.