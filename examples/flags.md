The global flags of mdscript
---

Here is the way to setup the global flags of mdscript. Simply create a code block and set its type to `@mdscript(--set-flags)`. For example,

<pre>
```@mdscript(--set-flags)
no-code: true
```
</pre>

The global options are written in `yaml` format. `mdscript` will remember the state of the options when executing the file from the top to the bottom. You may change them anytime in markdown file or reset to default with `--reset-flags`.

<pre>
```@mdscript(--reset-flags)
```
</pre>

By default, code blocks with `--set-flags` or `--reset-flags` will be removed from the output markdown file.

You may also add `yaml` type in the front to have better syntax highlighting in the markdown file.

<pre>
```yaml, @mdscript(--set-flags)
```
</pre>

Here are the default flags that used by `mdscript`:

```yaml, @mdscript(--set-flags)
# Remove the code block?
no-code: false
# Use custom script? null is to use the default script by languages.
# Check scripts directory to see the default scripts.
script: null
# The script lookup directory. Default is set to the directory that
# contains the input markdown file.
script-dir: null
```
