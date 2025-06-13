# Smart Resume Tailor

A simple, template-based resume generator using YAML for structured input and Python to render styled DOCX resumes.

## ✨ Features

- Use a clean YAML file to define your resume content
- Automatically render a .docx file using a pre-styled template
- Simple GUI interface to select your YAML file
- Easy to extend or modify for different resume styles

## 📦 Requirements

```bash
pip install python-docx pyyaml
```

## 🚀 How to Use

1. Place your YAML resume (example: `sample_resume.yaml`) in the same folder as the script and template.
2. Run the script:

```bash
python resume_renderer_gui.py
```

3. Click "Choose Resume YAML" and select your YAML file.
4. Your resume will be saved as a `.docx` file in the same folder.

## 🧾 Sample YAML Structure

```yaml
resume:
  header:
    name: Donald L. Coles
    contact:
      email: dlcoles@gmail.com
      phone: 713-503-6456
  start_with_why:
    content: |
      I believe clarity is the most powerful tool in a leader’s arsenal.

  who_i_am:
    content: |
      I’m a systems-first builder with a background that spans infrastructure, cloud, software, and strategy.

  how_i_work:
    blocks:
      - block_heading: Approaches & Methods
        list: [Agile, Waterfall, DevOps]
      - outro: I speak the language and support those who build.

  education:
    college:
      college_name: University Name
      degree_type: B.A.
      major_name: Philosophy
      year: 2009

  experience:
    section_title: What I’ve Done
    jobs:
      - job_title: Sr. Project Manager
        company_name: Sonic Automotive
        location: Remote
        date_start: July 2024
        date_end: Nov 2024
        summary: |
          Rebuilt team trust and delivered a failing PC refresh project ahead of schedule.
        bullets:
          - Reorganized project execution into Agile sprints
          - Reduced escalations by >50%
        punch_quote: More than just a project rescue—it was a full system reboot.
```

## 📝 License

MIT
