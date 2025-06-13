## ✅ สรุป Post Hoc Analysis

### 📌 **1. เมื่อใช้ One-way ANOVA**

(ใช้ข้อมูลแบบ **parametric**)

* 🔎 **ใช้ Post Hoc เพื่อเปรียบเทียบเป็นรายคู่ (pairwise)** เช่น:

  * กลุ่ม A vs B
  * กลุ่ม A vs C
  * กลุ่ม B vs C

* 📘 **Post Hoc ที่นิยม**:

   * Tukey's HSD
   *  Bonferroni
   *  Scheffé**

---

### 📌 **2. เมื่อใช้ Kruskal–Wallis test**

(ใช้ข้อมูลแบบ **non-parametric**)

* ❗ Kruskal–Wallis บอกแค่ว่า "มีความแตกต่างบางคู่" แต่ไม่บอกว่าคู่ไหน
* 🔍 **Post Hoc ที่ใช้**:

  * **Dunn’s test**
  * **Conover test**

---

### 📊 ตัวอย่างใน Jamovi:

หลังจากทำ ANOVA หรือ Kruskal–Wallis แล้ว:

1. ติ๊กที่เมนู “Post Hoc Tests”
2. เลือกกลุ่มที่ต้องการเปรียบเทียบ
3. เลือกประเภท correction (Tukey, Bonferroni, ฯลฯ)
4. โปรแกรมจะแสดงตารางเปรียบเทียบแต่ละคู่ พร้อม p-value

---

### 🔁 ตัวอย่างผลลัพธ์:

| Comparison | Mean Diff. | p-value (adjusted) |
| ---------- | ---------- | ------------------ |
| A vs B     | 2.4        | 0.021\*            |
| A vs C     | 0.9        | 0.310              |
| B vs C     | 1.5        | 0.045\*            |

→ \* มีเครื่องหมาย \* บอกว่าคู่นั้นต่างกันอย่างมีนัยสำคัญ
