# PAM - Proxy Api Manager
 Create proxy classes to manage your proxy urls

# Example
```
import ProxyApiManager as PAM

proxys = PAM.NewProxyApi("test")
print(proxys)
proxys.add_base_urls(["https://text1.com", "https://text2.com"])
proxys.add_base("https://text5.com")
print(proxys.get_base_url())
print(proxys.base_urls)
sub = "sub test"
proxys.add_sub(sub)
proxys.add_sub_url(sub, "/test1")
proxys.add_sub_urls(sub, ["/test2", "/test 3"])
print(proxys.get_sub_url(sub))
print(proxys.subs)
print(proxys.get_full_url(sub))
```