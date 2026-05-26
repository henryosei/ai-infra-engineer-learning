# Frequently Asked Questions (FAQ)

## General Questions

### What is this learning path about?

This is a comprehensive curriculum designed to help you become an AI Infrastructure Engineer. It covers everything from Docker and Kubernetes to cloud platforms, distributed training, and production ML systems.

### Who is this course for?

This course is for:
- Software engineers wanting to transition to AI infrastructure
- ML engineers who want to understand infrastructure better
- DevOps engineers looking to specialize in ML infrastructure
- Anyone interested in building and scaling ML systems

### What are the prerequisites?

**Required:**
- Python programming (intermediate level)
- Basic Linux/Unix command line
- Git basics
- Basic ML concepts

**Recommended:**
- Cloud platform awareness
- Docker basics
- Networking fundamentals

### How long does it take to complete?

- **Full-time** (40 hours/week): 12-15 weeks
- **Part-time** (10 hours/week): 50-60 weeks (~1 year)
- **Weekend** (20 hours/week): 25-30 weeks (~6-7 months)

Total: 500+ hours of content

### Is this course free?

The learning materials are completely free and open-source (MIT License). However, you may incur costs for:
- Cloud resources (most exercises fit within free tier limits)
- GPU instances for training projects (estimated <$100 total)

### Do I get a certificate?

Currently, this is a self-paced learning path without formal certification. However, completing all projects gives you a strong portfolio to showcase to employers.

---

## Technical Questions

### What programming languages do I need to know?

Primarily **Python**. You should be comfortable with:
- Functions and classes
- File I/O and error handling
- Package management (pip, venv)
- Basic async/await concepts

### Which cloud provider should I use?

Ideally, all three (AWS, GCP, Azure) as Module 02 covers each. However, you can start with any one:
- **AWS**: Most popular in industry, extensive ML services
- **GCP**: Strong ML/AI focus, good for experimentation
- **Azure**: Growing fast, good for enterprise

All have free tier or credits for new users.

### Do I need a GPU?

**For local development:** No, most exercises work on CPU.

**For training projects:** You'll need GPU access, but you can use:
- Cloud GPU instances (AWS, GCP, Azure)
- Google Colab (free tier available)
- Kaggle notebooks (free GPU access)

### What if I get stuck on an exercise?

1. Re-read the lesson material
2. Check the FAQ (you're here!)
3. Search existing [GitHub Issues](https://github.com/ai-infra-curriculum/ai-infra-engineer-learning/issues)
4. Ask in [GitHub Discussions](https://github.com/ai-infra-curriculum/ai-infra-engineer-learning/discussions)
5. Open a new issue with the `question` label

### Can I skip modules?

While the curriculum is designed to be progressive, you can skip modules if you already have the knowledge. However:
- Complete the quiz to verify your understanding
- Make sure you have the prerequisite skills for later modules

---

## Project Questions

### How do I know if my project is correct?

Since these are learning projects with code stubs:
1. All tests should pass (when you implement the TODOs)
2. The application should run without errors
3. Compare your implementation against best practices in the lessons
4. Share your code in Discussions for community feedback

### Can I use different technologies than suggested?

Yes! The stubs provide one approach, but you're encouraged to:
- Try alternative frameworks or libraries
- Implement additional features
- Optimize for different requirements

Share your alternative implementations in Discussions!

### Should I complete all projects?

**Yes**, if you want the full learning experience. Each project reinforces different concepts:
- Project 01: Foundations (serving, Docker, K8s)
- Project 02: Distributed training
- Project 03: MLOps pipelines
- Project 04: Auto-scaling systems
- Project 05: Complete ML platform

### Can I add projects to my portfolio?

Absolutely! All project code you write is yours. These projects make excellent portfolio pieces for job applications.

---

## Cloud & Cost Questions

### How much will cloud resources cost?

**Estimated total cost:** <$100 if you exceed free tier limits.

**Cost breakdown:**
- Module 01-02 (AWS/GCP/Azure basics): Free tier
- Module 03-04 (Kubernetes): ~$20
- Module 05-06 (Distributed training): ~$30-50
- Module 07-10 (Production systems): ~$20-30

**Cost-saving tips:**
- Use free tier whenever possible
- Shut down resources when not in use
- Use spot/preemptible instances (60-90% cheaper)
- Set billing alerts

### How do I avoid unexpected cloud bills?

1. **Set up billing alerts** immediately (recommended: $10, $25, $50)
2. **Shut down resources** after each session
3. **Use cloud budget tools**:
   - AWS Budgets
   - GCP Budget Alerts
   - Azure Cost Management
4. **Monitor usage daily**
5. **Use auto-shutdown scripts** (provided in lessons)

### Can I complete the course without cloud access?

Module 01 can be completed locally. However, Modules 02+ require cloud access for:
- Cloud storage and networking
- Managed ML services
- Kubernetes clusters
- Distributed training

You can use free tier/credits to minimize costs.

---

## Career Questions

### What jobs can I get after completing this?

You'll be qualified for:
- **AI Infrastructure Engineer** ($120k-$180k)
- **ML Platform Engineer** ($130k-$190k)
- **MLOps Engineer** ($110k-$170k)
- **Senior Cloud Engineer** (ML focus) ($130k-$200k)

### How does this compare to a bootcamp or degree?

**Advantages:**
- Free and open-source
- Self-paced
- Hands-on, project-based
- Industry-aligned curriculum

**Considerations:**
- No formal certification
- Requires self-discipline
- No instructor support (community-supported)
- No career placement services

### What should I do after completing this?

1. **Build your portfolio**: Publish your projects on GitHub
2. **Write about it**: Blog about what you learned
3. **Contribute back**: Help improve this curriculum
4. **Network**: Join ML infrastructure communities
5. **Apply for jobs**: Use your portfolio to demonstrate skills
6. **Keep learning**: Technology evolves rapidly

### Should I contribute to open source?

**Yes!** Contributing to this repository or other ML infrastructure projects:
- Demonstrates your skills
- Builds your network
- Helps you learn
- Looks great on your resume

---

## Content Questions

### Why are there TODOs in the code?

The code stubs with TODOs are intentional! They:
- Guide your implementation
- Provide hints and best practices
- Allow you to learn by doing
- Let you take ownership of the code

Complete solutions are available in the separate solutions repository.

### Where are the video tutorials?

This is a text-based curriculum. Benefits:
- Self-paced (skim or deep-dive as needed)
- Easy to search and reference
- Accessible (no bandwidth requirements)
- Can be translated

Video tutorials may be added in the future.

### Can I translate this to another language?

Yes! We welcome translations. See [CONTRIBUTING.md](../CONTRIBUTING.md) for guidelines.

### How often is the content updated?

The curriculum is actively maintained:
- **Quarterly updates**: New tools and best practices
- **Bug fixes**: As reported by community
- **Content improvements**: Based on feedback
- **New modules**: As technology evolves

---

## Community Questions

### How can I get help?

1. **Read documentation**: Lessons, README, this FAQ
2. **Search issues**: Someone may have asked already
3. **GitHub Discussions**: Ask the community
4. **Open an issue**: For bugs or unclear content

### How can I contribute?

See [CONTRIBUTING.md](../CONTRIBUTING.md) for detailed guidelines. Ways to contribute:
- Fix typos or errors
- Improve explanations
- Add examples or exercises
- Review pull requests
- Help answer questions
- Share your experience

### Is there a community chat?

[GitHub Discussions](https://github.com/ai-infra-curriculum/ai-infra-engineer-learning/discussions) is the supported channel today. Real-time chat (Slack/Discord) and recurring office hours are not currently scheduled — open a Discussion if you'd like to coordinate a study group.

### Can I share my progress?

Yes! We encourage it:
- Share in GitHub Discussions
- Tag #AIInfraLearning on social media
- Write blog posts about your journey
- Create videos of your projects

---

## Troubleshooting

### Docker permission denied

```bash
# Add your user to docker group
sudo usermod -aG docker $USER
newgrp docker
```

### Python import errors

```bash
# Activate virtual environment
source venv/bin/activate

# Reinstall dependencies
pip install -r requirements.txt
```

### Kubernetes connection refused

```bash
# Start minikube
minikube start

# Verify
kubectl get nodes
```

### AWS CLI not configured

```bash
# Configure AWS CLI
aws configure

# Enter your:
# - Access Key ID
# - Secret Access Key
# - Default region (e.g., us-east-1)
# - Output format (json)
```

### Out of disk space

```bash
# Clean Docker
docker system prune -a

# Clean pip cache
pip cache purge

# Check disk usage
df -h
```

---

## Still Have Questions?

- **Search existing**: [GitHub Issues](https://github.com/ai-infra-curriculum/ai-infra-engineer-learning/issues)
- **Ask community**: [GitHub Discussions](https://github.com/ai-infra-curriculum/ai-infra-engineer-learning/discussions)
- **Report bug**: Open a new [issue](https://github.com/ai-infra-curriculum/ai-infra-engineer-learning/issues/new)

---

**Didn't find your answer? Open a discussion or issue!**
