# My Resume

An interactive resume editor built with Claude.

I recently wanted to refresh my resume but the thought of fighting LibreOffice formatting lead me to spend a few hours experimenting using Claude to import my formatting I've used over the years to provide a rich interactive editor to make adjustments. 

Access the app at https://rdlaitila.github.io/myresume

No license or warrantee provided.

# Claude's Docs

## Overview
An interactive, single-file HTML resume editor that provides a split-panel interface with a live-preview of your professional resume. All data is stored locally in your browser with automatic versioning and no server requirements.

## Key Features

### Core Functionality
- **Split-Panel Editor**: Real-time editing on the left, formatted resume preview on the right
- **Print/PDF Export**: Professional print layout optimized for US Letter (8.5" × 11")
- **Local Storage**: All data persists in browser localStorage with automatic saves
- **Version History**: Automatic versioning with 50-version limit, navigate between versions, and branch/rename support
- **Share Links**: Generate shareable links with optional password protection (data encoded in URL)

### Dynamic Content Sections
- **Personal Info**: Name and tagline with customizable contact information (phone, email, LinkedIn, GitHub, etc.)
- **Professional Summary**: Free-form text area for your career summary
- **Flexible Section Types**:
  - **Subject Areas**: Labeled subsections (e.g., "Tools & Tech" with subsections for Languages, Frameworks, etc.)
  - **Word Cloud**: Bullet-point keyword lists (e.g., "Industry Knowledge")
  - **Work History**: Job experiences with company, title, date range, and descriptions
  - **Project List**: Notable projects with status, tags, URLs, and descriptions

### Data Management
- **Schema Versioning**: Built-in migration system (currently v3) automatically upgrades old resume formats
- **File Operations**: Save/load resume files as JSON, download copies
- **Collapsible Sections**: All editor sections collapse/expand for easier navigation
- **Drag-to-Reorder**: Move sections and items up/down with arrow buttons

### AI Integration
- **Chat Interface**: Optional AI assistant with floating chat button
- **Provider Support**: Configure OpenAI, Anthropic, or custom API providers
- **Context-Aware**: AI can help edit resume content with full access to current data

## Usage
1. Open `resume-editor.html` in a web browser
2. Choose "Create New Resume" or "Load Existing Resume"
3. Edit content in the left panel and watch the preview update in real-time
4. Click "Print / Save as PDF" to export
5. All changes are automatically saved to browser storage

## Technical Details
- **Zero Dependencies**: Pure vanilla JavaScript, HTML, and CSS
- **Responsive Design**: Adapts for different screen sizes (hides editor panel on mobile/print)
- **Data Schema**: JSON-based with version migration support
- **Browser Compatibility**: Works in all modern browsers with localStorage support