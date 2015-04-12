bandit6
=======
For next level see: http://overthewire.org/wargames/bandit/bandit7.html

```bash
ssh bandit6@bandit.labs.overthewire.org
  password:< DXjZPULLxYr17uwoI01bNLQbtFemEgo7

cat $(find / -type f -size 33c -user bandit7 -group bandit6  2>/dev/null )
  > HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

```
Next: [bandit7.md](bandit7.md)
