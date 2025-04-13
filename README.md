# Sistem-Pakar

# Added 4 new rules:
```python
@Rule(Fact(fever=True) & Fact(fatigue=True) & Fact(joint_pain=True))
  def dengue(self):
    print("Diagnosis: You may have Dengue Fever.")

  @Rule(Fact(cough=True) & Fact(breathing_difficulty=True) & Fact(chest_tightness=True))
  def asthma(self):
    print("Diagnosis: You may have Asthma.")

  @Rule(Fact(sneezing=True) & Fact(runny_nose=True) & Fact(itchy_eyes=True))
  def allergy(self):
    print("Diagnosis: You may have an Allergy.")

  @Rule(Fact(fever=True) & Fact(cough=True) & Fact(loss_of_smell=True))
  def covid19(self):
    print("Diagnosis: You may have COVID-19.")
```
# Added 4 new question:
```python
return{
    "joint_pain": ask_question("Do you have joint pain?"),
    "chest_tightness": ask_question("Do you feel chest tightness?"),
    "itchy_eyes": ask_question("Do you have itchy eyes?"),
    "loss_of_smell": ask_question("Have you lost your sense of smell?")
}
```
