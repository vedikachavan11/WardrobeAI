# 👗 WardrobeAI

### Your Personal AI-Powered Wardrobe Assistant

WardrobeAI is a web-based wardrobe management and outfit recommendation platform designed to make everyday fashion decisions easier. It helps users organize their clothing and discover outfit ideas based on occasions, weather conditions, and personal preferences.

## ✨ Features

- **Wardrobe Management:** Organize and manage clothing items.
- **Smart Outfit Recommendations:** Discover outfit combinations suited to different occasions.
- **Weather-Based Suggestions:** Choose outfits according to weather conditions.
- **Personalized Experience:** Tailor recommendations to individual preferences.
- **User Authentication:** Access a personalized experience through secure sign-in.

## Architecture diagram

flowchart TD
    A["GitHub Repository URL"] --> B["Repository Validation"]
    B --> C["Clone Repository"]
    C --> D["Filter Source Files"]
    D --> E["AST Parsing and Semantic Chunking"]
    E --> F["Generate Embeddings"]
    F --> G[("Supabase PostgreSQL + pgvector")]
    
    H["Client / Frontend"] --> I["FastAPI REST Service"]
    I --> J{"Request Type"}
    J -->|POST /index| B
    J -->|POST /search| K["Embed Search Query"]
    K --> L["Vector Similarity Search"]
    G --> L
    L --> M["Retrieve Relevant Code Chunks"]
    M --> N["Return Results with File Paths and Line Numbers"]
    N --> H
    
    style A fill:#EDE9FE,stroke:#7C3AED,color:#111827
    style I fill:#DBEAFE,stroke:#2563EB,color:#111827
    style G fill:#D1FAE5,stroke:#059669,color:#111827
    style E fill:#FEF3C7,stroke:#D97706,color:#111827
    style N fill:#FCE7F3,stroke:#DB2777,color:#111827


## 🛠️ Tech Stack

- **Frontend:** React.js, Vite
- **Backend & Database:** Supabase
- **Weather Integration:** Weather API
- **Languages:** JavaScript, HTML, CSS

## 🎯 Project Goal

The goal of WardrobeAI is to simplify wardrobe management, reduce the time spent deciding what to wear, and help users make better use of their existing clothing.

## 🚀 Project Status

Under development. Features and functionality may change as development progresses.

## 👩‍💻 Author

**Vedika Chavan**

GitHub: [@vedikachavan11](https://github.com/vedikachavan11)

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
