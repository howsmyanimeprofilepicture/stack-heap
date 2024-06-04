---
marp: true
header: "Source: https://courses.engr.illinois.edu/cs225/fa2022/resources/stack-heap/"

---

![height:550px](1.png)

1. Allocate Cube `c` for `CreateCube`.

---

![height:550px](2.png)

2. Deallocate stack memory of `CreateCube` and return address of `c`.

---

![height:550px](3.png)

3. Allocate pointer `c` for `main` and store the returned value. Notice that the stack memory of `CreateCube` is **overwritten**.

---

![height:550px](4.png)

4. Allocate stack memory for `getVolume` and calculate volume using the width of `c`. Since the width of `c` is **corrupted**, the volume is also **incorrect**.


---

![height:550px](5.png)

5. Deallocate memory of `getVolume`. Allocate `r` for `main` to store the return value of `getVolume`.

---

![height:550px](6.png)

6. Allocate stack memory for `getSurfaceArea` and calculate surface area using the width of `c`. Similar to `getVolume`, the surface area calculated will be incorrect.

---

![height:550px](7.png)

7. Deallocate memory of `getSurfaceArea`. Allocate `v` for main to store the return value of `getSurfaceArea`.

---

![height:550px](8.png)

8. Deallocate the stack memory of `main` and return `0`
