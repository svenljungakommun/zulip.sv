# Zulip Swedish Translation (sv)

**Full Swedish translation file for Zulip**  
Maintainer: Svenljunga kommun  

---

## Overview

`json/translations.json` is a complete Swedish translation file for [Zulip](https://zulip.com), the open-source team chat platform.  

All user interface strings have been translated into clear and consistent Swedish. Keys and variables remain unchanged; only values have been translated. The translation aims to provide a user-friendly experience for Swedish municipalities, public sector organizations, companies, and communities.

---

## Features

- 🌍 100% Swedish coverage of the Zulip UI  
- 🔑 Keys and variables unchanged — values only translated  
- 📑 Clear, plain Swedish terminology:
  - **Channel** → *Kanal*  
  - **Topic** → *Ämne*  
  - **Notifications** → *Notiser*  
  - **Inbox** → *Inkorg*  
- 🛠 Includes:
  - Administrative UI texts  
  - Error messages  
  - System notifications  
  - Help texts  

---

## Installation

### Non-container deployment

Copy the translation file into the Zulip locale directory:

```bash
cp json/translations.json /home/zulip/deployments/current/locale/sv/translations.json
````

Restart Zulip for changes to take effect.

---

### Docker deployment

Mount the translation file as a volume in your `docker-compose.yml`:

```yaml
zulip:
  volumes:
    - "<host-path>/translations.json:/home/zulip/deployments/current/locale/sv/translations.json"
```

Restart the Zulip container:

```bash
docker compose restart zulip
```

---

After installation, enable **Svenska (sv)** in:

```
Organization settings → Language
```

and reload your Zulip client.

---

## Example Snippet (`translations_sv.json`)

```json
{
  "Send": "Skicka",
  "Cancel": "Avbryt",
  "Inbox": "Inkorg",
  "Notifications": "Notiser",
  "Channel": "Kanal",
  "Topic": "Ämne"
}
```

---

## Notes

* All keys remain unchanged for compatibility with Zulip upstream.
* Swedish language pack can be maintained alongside official Zulip updates.
* Pull requests with corrections or improvements are welcome.

---

## Testing

You can test the translation by switching language in your Zulip web client:

```bash
Settings → Display settings → Language → Svenska
```

or by modifying server language configuration.

---

## License

Released under the **MIT License**, in line with Zulip’s open-source licensing.
You are free to use, modify, and distribute the translation as long as license information is preserved.
