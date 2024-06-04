---
marp: true
header: "Source: https://courses.engr.illinois.edu/cs225/fa2022/resources/stack-heap/"

---

![height:550px](1.png)

1. Allocate a `Cube` width `20` on the heap, allocate a Cube pointer `c` on `CreateCubeOnHeap`'s stack to store the address of the `Cube`.

---

![height:550px](2.png)

2. Deallocate stack memory for `CreateCubeOnHeap` and return the value of pointer `c`.

---

![height:550px](3.png)

3. Allocate `cube` on `main`'s stack and store the returned pointer.

---

![height:550px](4.png)

4. Call method `getVolume` on `cube`, which calculates the volume to be `8000`.

---

![height:550px](5.png)

5. Allocate double `v` to store the return value `8000`.

---

![height:550px](6.png)

6. Deallocate the `Cube` pointed by `cube`, notice that cube is **still pointing to invalid memory** on heap

---

![height:550px](7.png)

7. Set the value of `cube` to `nullptr`, which is `0`.

---

![height:550px](8.png)

8. Deallocate the stack memory of `main`.
