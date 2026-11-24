# Apps

Executable [script commands](./scripts.md) also appear in normal search. Scripts with arguments open a separate argument field; their output can stay inline or stream into the Script Output window.

Dupin finds the `.app` bundles in `/Applications`, `/System/Applications` and `~/Applications`, one folder deep (so `Utilities` is included). It also finds Finder at `/System/Library/CoreServices/Finder.app` and app bundles directly in `/System/Library/CoreServices/Applications`. Apps in the standard application folders take precedence when bundle names match.

An app matches by any name macOS knows it by:

- the name Finder shows, localized (システム設定 for System Settings on a Japanese Mac);
- its file name, when that differs;
- Spotlight's alternate names and keywords: ChatGPT answers to "Codex", its former name, System Settings to "System Preferences", Safari to "browser".

When an app matches through one of those other names, the name shows before its folder in the result.
