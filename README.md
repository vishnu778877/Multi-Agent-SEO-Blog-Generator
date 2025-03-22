# Multi-Agent SEO Blog Generator

## System Architecture
The system is built using a **multi-agent architecture** with five agents:
1. **Research Agent**: Fetches trending HR topics from the web.
2. **Content Planning Agent**: Creates a structured outline for the blog post.
3. **Content Generation Agent**: Generates blog content using Hugging Face's GPT-2 model.
4. **SEO Optimization Agent**: Optimizes the content for SEO by adding keywords and formatting.
5. **Review Agent**: Proofreads and improves the content quality.

---

## Agent Workflow
1. **Research Agent**:
   - Fetches trending HR topics from Google News.
   - If no topics are found, it defaults to a generic topic ("HR Trends").

2. **Content Planning Agent**:
   - Creates a structured outline with an introduction, main points, and conclusion.

3. **Content Generation Agent**:
   - Uses GPT-2 to generate blog content based on the outline.

4. **SEO Optimization Agent**:
   - Adds `<strong>` tags to keywords (e.g., "HR" and "trending") for SEO.

5. **Review Agent**:
   - Proofreads and improves the content quality (currently a placeholder implementation).

---

## Tools and Frameworks
- **Python 3.x**: The programming language used for development.
- **Hugging Face Transformers**: For text generation using the GPT-2 model.
- **BeautifulSoup4**: For web scraping trending topics from Google News.
- **Markdown**: For converting the final blog post to Markdown format.
- **Requests**: For making HTTP requests to fetch data from the web.

---

## Installation and Execution

### Step 1: Open in Google Colab
1. Open the notebook in Google Colab:  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vishnu778877/Multi-Agent-SEO-Blog-Generator/blob/main/multi_agent_blog_generator.ipynb)

2. Alternatively, clone the repository:
   \`\`\`bash
   git clone https://github.com/vishnu778877/Multi-Agent-SEO-Blog-Generator.git
   cd Multi-Agent-SEO-Blog-Generator
   \`\`\`

### Step 2: Install Dependencies
Run the following command in Google Colab or your local environment:  
`!pip install transformers requests beautifulsoup4 markdown`

### Step 3: Run the Code
- Open `multi_agent_blog_generator.ipynb` in Google Colab or Jupyter Notebook.
- Run all cells sequentially.

### Step 4: View the Output
The final blog post will be saved as `blog_post.md` in the project directory.

---

## Repository Structure
Multi-Agent-SEO-Blog-Generator/

├── multi_agent_blog_generator.ipynb  # Main Jupyter notebook

├── blog_post.md                      # Generated blog post

├── requirements.txt                  # List of dependencies

└── README.md                         # This file
