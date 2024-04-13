<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  
  tR += "---"
%>
Created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
Modified: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
Alias: 
Tags: Meeting
---

Related to: 

# 🏠 Logistics
Date: <% tp.file.creation_date("YYYY-MM-DD") %>
Time: <% tp.file.cursor(1) %>
Location: 

# 🗣️ Participants
- Sascha D. Kasper
- 

# 📅 Agenda


# 🗒️ Notes


# ✅ Action Items

## Mine
- [ ] 

## Others
- [ ] 