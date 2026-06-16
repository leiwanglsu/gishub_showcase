# Risk and Governance (Public Summary)

## Governance Principle
All current outputs are preliminary and non-certification. This is not a temporary limitation—it is a first-class design constraint that shapes every workflow, template, and decision gate.

## Why Governance-First Design Matters
Preliminary elevation outputs can appear authoritative and numerically precise. Without strong governance controls, stakeholders can easily (and unintentionally) overinterpret results or use them beyond their intended scope. Governance-first design prevents this by making limitations explicit and inescapable.

## Primary Risk Categories

### 1. Evidence Completeness Risk (HIGH IMPACT)
**Risk**: Using preliminary outputs as evidence for certification-grade decisions without control/checkpoint validation.

**Current State**: 
- No GPS-surveyed control points or independent checkpoints collected
- Comparative benchmarking only; no absolute ground truth tie
- Results are internally consistent but not GPS-verified

**Mitigation**:
- All outputs explicitly state: "Preliminary and non-certification"
- Readiness states prevent promotion without control/checkpoint evidence
- Staged gates block certification-oriented release paths
- Documented path to evidence collection in next phase

**Next Steps**: 
- Collect GPS-surveyed control points and checkpoints in pilot sites
- Recompute residuals against verified field measurements
- Validate performance across 5-10 additional sites

### 2. Interpretation Risk (HIGH IMPACT)
**Risk**: Stakeholders mistake screening results for certification evidence.

**Current State**:
- Outputs are report-ready and visually persuasive
- Non-technical audiences may not understand "draft" status
- Governance controls can be overlooked if not prominent

**Mitigation**:
- Non-certification language appears in every external-facing document
- Readiness states use explicit terminology (draft/pending-control/reviewed)
- Training materials emphasize scope boundaries
- Template language prevents accidental mis-framing

**Next Steps**:
- Expand stakeholder communication program
- Document common misinterpretations and how to address them
- Build feedback loop to capture stakeholder questions

### 3. Operational Consistency Risk (MEDIUM IMPACT)
**Risk**: Results vary across different sites or operators due to inconsistent capture methods or processing.

**Current State**:
- Deterministic processing established for server-side logic
- Capture method standards documented but not yet enforced at field level
- Single pilot site tested; multi-site variability unknown

**Mitigation**:
- Intake validation flags anomalous capture parameters
- Deterministic workflows ensure reproducibility
- Capture method documentation (distance, tripod, duration, angle)
- Documented SOP for field teams

**Next Steps**:
- Expand validation to 5-10 sites with varied capture conditions
- Build performance sensitivity model (how capture method affects results)
- Develop field training and certification program

### 4. Quality Variability Risk (MEDIUM IMPACT)
**Risk**: Mobile LiDAR quality varies with device, environment, capture technique.

**Current State**:
- iPad LiDAR tested; iPhone and other devices not yet validated
- Good performance in open areas; degraded performance in dense vegetation
- Capture technique (tripod vs. handheld) not yet quantified

**Mitigation**:
- Benchmarking identifies quality divergence hotspots
- QA state communicates fitness-for-purpose
- Comparative analysis supports relative quality assessment
- Hotspot mapping guides targeted recapture

**Next Steps**:
- Systematic device and environment testing
- Build quality sensitivity models
- Document device/environment trade-offs

### 5. Security and Data Governance Risk (MEDIUM IMPACT)
**Risk**: Capture data or internal analysis could be misused if access is not controlled.

**Current State**:
- Local device storage only; no sensitive data in current demo
- iOS app under assessment; data protection features planned
- Public showcase repo contains only safe materials

**Mitigation**:
- Data classification and access controls (planned for next phase)
- Audit logging for all significant operations
- Non-certification disclaimers on all external outputs
- Public repo excludes operational data and internal reports

**Next Steps**:
- Develop data governance policy
- Implement formal access control and audit logging
- Plan encryption and secure transport for scaled deployment

## Mitigation Posture

### Three-Layer Control Strategy

**Layer 1: Prevent Bad Data (Intake Controls)**
- Validate package completeness and metadata quality
- Reject incomplete or malformed data before processing
- Flag anomalous capture parameters for review

**Layer 2: Preserve Integrity (Processing Controls)**
- Deterministic workflows ensure reproducibility
- Every decision is traceable to specific inputs
- Version all artifacts with timestamps and scan IDs

**Layer 3: Communicate Limitations (Release Controls)**
- Explicit readiness states (draft/pending-control/reviewed)
- Non-certification language on all stakeholder-facing outputs
- Staged gates prevent premature external sharing
- Templates enforce consistent communication

### Governance Principles
1. **Transparency**: Every limitation is visible; nothing is hidden
2. **Auditability**: Every decision can be reconstructed from records
3. **Defensibility**: Governance choices are documented and justified
4. **Extensibility**: Current controls extend cleanly to certification-final workflows

## Risk Monitoring and Escalation

**Monitoring Triggers**:
- Repeated intake warnings on the same field condition
- High hotspot concentration in benchmark results
- Persistent draft state despite refinement attempts
- Any evidence that stakeholders are treating outputs as certification

**Escalation Actions**:
- Pause release until root cause is understood
- Document issue in audit trail
- Rerun analysis with corrected parameters
- Update field or operational procedures
- Report status to stakeholders with mitigation plan

## Governance Roadmap

**Current Phase**: Pilot readiness with explicit non-certification boundaries
**Next Phase**: Control/checkpoint integration with certification-path planning
**Future Phase**: Certified elevation issuance with licensed professional sign-off

Each phase builds on the governance framework of the previous one without requiring redesign.
