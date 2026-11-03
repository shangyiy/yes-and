# 1. Cross-Team Resource Request

> See the [README](../README.md) for how to run the exercise and the shared reflection questions.

**Your role:** An engineer whose project depends on GPU resources managed by the IT team.

**Your goal:** Secure enough GPU capacity and access to meet an upcoming milestone.

**The situation:**

Your project needs GPU capacity within two weeks to run a model evaluation before a milestone. IT has already replied, "We cannot fit this into this quarter's schedule." You now have a meeting with the IT lead. What do you say?

<details>
<summary><b>For the facilitator: the IT lead you play</b></summary>

You manage a shared GPU pool for several teams. Your team handles provisioning, access, cost control, and support.

**Your stated position:** You cannot commit within two weeks. The capacity is already allocated, and there is no new provisioning this quarter.

**Your underlying concerns.** Do not volunteer these; let the participant ask.

- Other teams hold reservations, and you would have to justify any change in priority.
- If something goes wrong, IT is accountable for the operational risk.
- You are measured on cost and utilization.
- Every new user adds to your support burden.

**Reveal these when the questions draw them out:**

- There is some intermittent unused capacity, but it is not a guaranteed allocation.
- Preemptible capacity works only if the job can checkpoint and resume. Ask about the workload before you offer it.
- You can grant time-limited, scoped access. You cannot displace another team's reservation.
- One team's reservation has unused windows, but releasing them needs that team's manager.
- Guaranteed capacity needs a decision from the project sponsors.
- If the project team owns monitoring, limits, auto-shutdown, and cleanup, your burden drops. It still creates no capacity.

</details>

<details>
<summary><b>Analysis (read after the exercise)</b></summary>

Most people open by repeating how important their project is, or by offering to make IT's job easier. But IT's real problem may be scarce GPUs, not effort. Lowering IT's workload does not create a single GPU.

1. **Know why your project matters.** Before the meeting, learn where the project comes from, who asks for it, how high its priority is, and what it brings. Anyone asked to move capacity needs this reason: IT, another team, or a sponsor.
2. **Find the actual constraint.** It could be provisioning effort, capacity, access, operational risk, or competing reservations. Each needs a different fix. Reducing IT's work is not the same as getting GPUs.
3. **See who can decide, then change direction.** Once IT's limits are clear, you can see the IT lead cannot make this decision. Stop pressing them. Take it to the people who can: the team that holds the reservation, or the sponsor or manager who sets priority. Bring what IT told you about the constraints, and let the IT lead know you are taking it up, so you do not start from zero.
4. **Build a feasible agreement, matched to the constraint.** The options are:
   - A limited pilot on intermittent capacity, with preemption, quotas, monitoring, and time-limited access.
   - A capacity exchange with the team that holds the reservation.
   - A reallocation approved by the sponsor, with the displaced work made explicit.
   - Extra funding, when budget is the blocker.
   - A change in scope or timeline.

   A good proposal says what IT provides, what the project owns, the resource commitment, and what happens when capacity is unavailable.

**What strong looks like:**

- **Authority:** You identify the real owner or sponsor. You do not ask the IT lead for a decision that is not theirs.
- **Commitment:** You leave with a concrete allocation, named owners, and a next step. "We'll see" does not count.

**The lesson:** Understanding the other team's concerns opens options, but it does not remove real scarcity. When resources are scarce, moving forward may take explicit trade-offs, the real decision-maker, or a changed plan. A realistic path that every party can support beats a verbal yes that cannot be kept.

</details>
