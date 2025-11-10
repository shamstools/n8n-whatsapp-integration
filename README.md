## 🧠 WhatsApp AI Assistant (n8n + OpenRouter / OpenAI)

### 📋 Description

This template shows how to connect **n8n** with **WhatsApp** and integrate it with **OpenRouter** or **OpenAI API** to create an intelligent AI agent that replies directly inside WhatsApp.
Once you import the template into n8n and adjust a few settings, you’ll have an automated AI chatbot ready to respond instantly to messages.

---

### ⚙️ Requirements

* A working **n8n** instance (self-hosted or cloud).
* An active **WhatsApp Cloud API** account via Meta.
* A valid **OpenRouter** or **OpenAI API key**.

---

### 🚀 How to Use

1. **Download the Template**

   * Copy the file `whatsapp-ai-agent-template.json` from this repository or from the YouTube video link.

2. **Import into n8n**

   * In your n8n dashboard, go to:
     `Import > From File` and select the template file.

3. **Edit Sensitive Data (Very Important ⚠️)**
   After importing, open each node and update the following values:

   #### 🔐 Replace the following:

   | Field                  | What to do                                      | Example                                      |
   | ---------------------- | ----------------------------------------------- | -------------------------------------------- |
   | `webhookId`            | Replace with your own Webhook ID from n8n       | `"webhookId": "YOUR_WEBHOOK_ID"`             |
   | `credentials.id`       | Remove or replace with `"REPLACE_WITH_YOUR_ID"` | `"id": "REPLACE_WITH_YOUR_ID"`               |
   | `phoneNumberId`        | Replace with your WhatsApp number ID from Meta  | `"phoneNumberId": "YOUR_PHONE_NUMBER_ID"`    |
   | `recipientPhoneNumber` | Use your own or a test number                   | `"recipientPhoneNumber": "YOUR_TEST_NUMBER"` |

   🔸 **Note:** Never share these values publicly, as they are tied to your personal accounts.

4. **Connect Your Accounts**

   * Link the **WhatsApp Trigger** and **Send Message** nodes to your WhatsApp API credentials.
   * Link the **OpenRouter Chat Model** node to your API key from [OpenRouter.ai](https://openrouter.ai/) or [OpenAI](https://platform.openai.com/).

5. **Test the Workflow**

   * Activate the workflow and configure the Webhook URL in Meta settings.
   * Send a message from WhatsApp to see the AI respond instantly ✨

---

### 🧩 Template Components

| Node                      | Function                                         |
| ------------------------- | ------------------------------------------------ |
| **WhatsApp Trigger**      | Receives new messages from WhatsApp              |
| **AI Agent**              | Sends the incoming text to the AI model          |
| **OpenRouter Chat Model** | Processes the message using OpenRouter or OpenAI |
| **Send Message**          | Sends the AI response back to WhatsApp           |
| **Sticky Note**           | Contains notes and template credits              |

---

### 💡 Tips for a Professional Touch

* Rename the workflow to `WhatsApp AI Assistant`.
* Add a logo or banner to the repository.
* Use a short GitHub description such as:

  > Connect n8n with WhatsApp and OpenRouter/OpenAI to build an AI assistant that chats directly inside WhatsApp.

---

### 👨‍💻 Created by

**HoloolPro**
📺 [YouTube Channel](https://www.youtube.com/@HoloolPro)
📧 [shamstutos@gmail.com](mailto:shamstutos@gmail.com)

---
