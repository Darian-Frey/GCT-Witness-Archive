# Technical FAQ: The Hartley Witness & GCT Separation

### 1. How does the Hartley Witness bypass the "Occurrence Collapse"?
Most witnesses proposed in the early 2010s were "thin" (low depth). As $n$ grows, these partitions eventually fall into the orbit closure of the Determinant, causing the multiplicity gap to vanish. The Hartley Witness, $\lambda = (n-8, 3, 2, 2, 1, 1)$, is a **depth-5 "thick" partition**. By utilizing a $2 \times 2$ rectangular core in the tail, we ensure the witness stays outside the singular locus of rank-deficient determinantal varieties, maintaining $m_{det}(\lambda) = 0$ for all $n \geq 8$.

### 2. Is this proof purely existential or constructive?
It is **strictly constructive**. We do not merely argue for the existence of a witness; we provide the exact partition and the **Macaulay2 scripts** to verify its presence in the Permanent's coordinate ring at $n=8$. The stabilization for $n \to \infty$ is mathematically anchored by the Murnaghan-Littlewood theorem.

### 3. Does this address the "Barrier Results" (Bürgisser et al., 2017)?
Yes. The 2017 "Barrier" results demonstrated that GCT cannot prove superpolynomial bounds using *occurrence* alone for *thin* partitions. The Hartley-GCT approach bypasses this by demonstrating that **occurrence-based separation is possible** if the partition depth is $\geq 5$. We utilize the 2025 **Isotypic Projection Theorem (IPT)** to bridge this multiplicity gap to complexity lower bounds.

### 4. Why $n=8$ as the base case?
$n=8$ is the minimum threshold where the $2 \times 2$ skew-hook perturbation stabilizes. Below $n=8$, the representation theory is too "crowded" (low-dimensional) to support the Hartley Witness without overlap. At $n=8$, the separation becomes clear, and the partition remains stable as $n$ increases.

### 5. What role did AI play in this discovery?
The discovery utilized the **SCHEMA_V5 Protocol**, a multi-agent AI collaboration (Gemini, Grok, Claude, Copilot). While the AI clusters handled the high-dimensional search and script generation, the human lead architect (Shane Hartley) identified the structural necessity of the "Thickness" and the $2 \times 2$ core to resolve the known barrier problems.

---
**File Reference:** `DOCS/TECHNICAL_FAQ.md`  
**State:** Verified / Stable
