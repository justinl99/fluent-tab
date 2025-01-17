# Fluent New Tab

Tab mới theo phong cách Fluent Design của Microsoft

![image](https://user-images.githubusercontent.com/30421456/157072440-8a84a472-1a02-41c1-aec7-174fe0e98dd0.png)



Meant as a replacement for the default "New Tab" experience in Microsoft Edge, for all the Fluent Design afiocionados out there 🎨

<br>
<br>

## Configuration

Configuration is currently handled through a CLI interface. To use it, open the DevTools and enter one of the following commands in the Tab "Console", then confirm by pressing Enter:

### `backgroundImage.choose()`:

Chọn một tệp để làm hình nền mới. Kích cỡ không quá 2MB.

### `backgroundImage.reset()`:

Xóa hình nền tự chọn của bạn và sử dụng lại hình nền mặc định.

### `siteConfig.addSite()`:

Add a new thumbnail for a given URL, which you can insert between the two parentheses. Needs to be quoted and a full valid URL including the protocol.  
E.g. `siteConfig.addSite("https://jonaskuske.com")` 🌐

### `siteConfig.removeSiteAtPosition()`:

Remove the site(s) at the given position(s), which you can insert between the parentheses, separated by commas.  
E.g. `siteConfig.removeSiteAtPosition(1)` will delete the first thumbnail and `siteConfig.removeSiteAtPosition(2,5,8)` will delete the 2nd, 5th and 8th site.

### `siteConfig.reset()`:

Undo thumbnail customizations and use the 8 default sites.

<hr>

**A more robust configuration with an actual UI will follow once I have the time for it.**

&nbsp;  
&nbsp;

### `_reset()`:

⚠ Clear all caches and reset everything. Only use this if you run into issues.
