# SWE_2021_41_2024_2_week_6

### Week 4 Assignment
---
[Week 4 Assignment Link](https://github.com/sinakivi/SWE_2021_41_2024_2_week_4/)

<pre>
  <code>
def isHappy(n, s=set()):
  if n == 1:
    return True
  elif n in s:
    return False

  i = 0
  t = n
  while t > 0:
    i += (t % 10) ** 2
    t = ((t - (t % 10)) / 10)

  s.add(n)
  return isHappy(i, s)


print(isHappy(1111111111))
print(isHappy(11111111111))
  </code>
</pre>

> ### Description
> Check recursively if n is 1 or already visited
> <br>
> Add n to visited set before calling self

### Week 5 Assignment
---

> <pre><code>docker exec ossp-container cat /etc/os-release</code></pre>
> - Check OS version

> <pre><code>docker exec ossp-container git --version</code></pre>
> - Check Git version

> <pre><code>docker exec ossp-container python3 --version</code></pre>
> - Check Python version

> <pre><code>docker inspect --format="{{ .HostConfig.Binds }}" ossp-container</code></pre>
> - Check binded volumes
