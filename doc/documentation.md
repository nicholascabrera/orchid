# Orchid Development Documentation
This document is a compendium of the design approach that the team will take towards the project.

## Deliverables

- [ ] Define Core Values
    - [ ] 
- [ ] Threat Model
    - [ ] Determine what Orchid guarantees and what it can't
- [ ] Define Scope
    - [ ] OS
    - [ ] UI
    - [ ] Whats being stored/protected?
    - [ ] Supported features
    - [ ] Storage location
    - [ ] Crypto suites
    - [ ] KDFs
- [ ] What is not in Scope
- [ ] Diagrams
    - [ ] Architectural Model (Layered)
        - [ ] Layer + Trust Boundaries
        - [ ] Logical Flow of Data
        - [ ] Where are logs stored? What can they log?
    - [ ] Vault Format
        - [ ] Filesystem Structure
        - [ ] Header Format
            - [ ] Versioning Scheme
            - [ ] KDF Param Storage Scheme
            - [ ] Cipher Suite Metadata Storage
        - [ ] Entry Format
            - [ ] File Structure
            - [ ] Atomic Write Strategy
        - [ ] Integrity Verification Mechanism
    - [ ] Key Heirarchy Flow
        - [ ] Authentication flow
        - [ ] Entry Enc/Dec flow
        - [ ] Flow of keys from Master Pass to Encrypting Entries
        - [ ] Rekey process
    - [ ] Vault Corruption
      - [ ] Detection Strategy
      - [ ] Handling Strategy
- [ ] Select a License
- [ ] Decide the repository structure
- [ ] Decide coding standards
    - [ ] Mandatory testing - where? what?
    - [ ] PRs - who? how?
    - [ ] Style - clangd? docker + dev containers?
- [ ] CI Pipeline
    - [ ] Build + Compilation Checks
    - [ ] SAST
    - [ ] Testing
    - [ ] Environment
    - [ ] Coding Standard enforcement
- [ ] Public Identity
    - [ ] Arch Linux of Secrets Managers?
    - [ ] Who are we? What are we? What are we not?
    - [ ] Security Philosophy
    - [ ] Threat Model Summary
    - [ ] v0 Scope
    - [ ] WARNING: We are still unstable!
- [ ] Refine SECURITY.md
    - [ ] How to report vuln
        - [ ] What information needed for report?
    - [ ] Responsible Disclosure Policy
    - [ ] Contact Method
    - [ ] Proof of Concept needed?
- [ ] Orchid Versioning Strategy
    - [ ] Separate by domain?

At the end of the day, before coding starts, these are the things we need to get done. We need 1-3 non-negotiable tenets to guide our decisions in the future, and a serious engineering approach to secure software.