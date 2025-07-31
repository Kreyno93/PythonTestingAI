# Python Testing Demo with GitHub Actions

This project demonstrates automated testing using GitHub Actions with HTML report generation.

## 🚀 What This Demo Shows

- **Automated Testing**: Tests run automatically when you push code
- **Multiple Python Versions**: Tests across Python 3.9, 3.10, 3.11, and 3.12
- **HTML Reports**: Beautiful test reports generated automatically
- **Code Coverage**: Shows how much of your code is tested
- **GitHub Pages**: Reports published automatically to a website

## 📁 Project Structure

```
PythonTesting/
├── main.py                    # Our simple add function
├── test_main.py              # Test cases
├── requirements.txt          # Python dependencies
├── .github/workflows/
│   ├── test.yml             # Full-featured workflow
│   └── simple-test.yml      # Beginner-friendly workflow
└── README.md                # This file
```

## 🧪 The Tests

Our simple `add` function is tested with:
- ✅ Positive numbers: `add(2, 3) == 5`
- ✅ Negative numbers: `add(-2, -3) == -5`
- ✅ Zero values: `add(0, 5) == 5`
- ✅ Mixed signs: `add(-2, 3) == 1`
- ✅ Float numbers: `add(2.5, 3.1) == 5.6`

## 🔄 GitHub Actions Workflows

### 1. Simple Workflow (`simple-test.yml`)
**Perfect for beginners!**
- Runs on Python 3.12
- Creates HTML test report
- Easy to understand steps
- Great for learning

### 2. Advanced Workflow (`test.yml`)
**Production-ready features:**
- Tests multiple Python versions
- Generates coverage reports
- Deploys to GitHub Pages
- Includes notifications

## 🚀 How to Use

### Step 1: Push to GitHub
```bash
git add .
git commit -m "Add automated testing"
git push origin main
```

### Step 2: Watch the Magic! ✨
1. Go to your GitHub repository
2. Click on the "Actions" tab
3. Watch your tests run automatically
4. Download the HTML reports when complete

### Step 3: View Reports
- **Test Reports**: Download from the Actions artifacts
- **GitHub Pages**: Available at `https://yourusername.github.io/your-repo-name`

## 📊 What You'll See

### In the GitHub Actions Tab:
- ✅ Green checkmarks when tests pass
- ❌ Red X when tests fail
- 📊 Downloadable HTML reports
- ⏱️ Execution time for each step

### In the HTML Report:
- Beautiful visual dashboard
- Individual test results
- Code coverage metrics
- Professional formatting

## 🎓 Learning Outcomes

Students will learn:
1. **CI/CD Basics**: How automated testing works
2. **GitHub Actions**: Writing workflow files
3. **Test Automation**: Running tests on every code change
4. **Report Generation**: Creating professional test reports
5. **Multi-environment Testing**: Testing across Python versions

## 🛠️ Local Development

Run tests locally:
```bash
# Install dependencies
pip install -r requirements.txt

# Run tests with HTML report
pytest test_main.py -v --html=report.html --self-contained-html

# Run with coverage
pytest test_main.py --cov=main --cov-report=html
```

## 🔧 Customization

### Add More Tests
Edit `test_main.py` to add more test cases:
```python
def test_add_large_numbers():
    assert add(1000000, 2000000) == 3000000
```

### Modify Workflow
Edit `.github/workflows/simple-test.yml` to:
- Change Python version
- Add more steps
- Customize notifications

## 🌟 Best Practices Demonstrated

- **Descriptive test names**: Easy to understand what failed
- **Multiple test scenarios**: Edge cases and normal cases
- **Automated reporting**: No manual report generation
- **Version compatibility**: Testing across Python versions
- **Documentation**: Clear README and comments

## 🎯 Perfect for Teaching

This setup is ideal for:
- **Bootcamp students**: Learning modern development practices
- **CS courses**: Understanding automated testing
- **Workshops**: Hands-on CI/CD experience
- **Code reviews**: Professional development workflow

## 🚨 Troubleshooting

### Tests Failing?
1. Check the Actions tab for error details
2. Look at the test report artifacts
3. Verify your code matches the expected behavior

### No HTML Report?
1. Ensure `pytest-html` is installed
2. Check the workflow file syntax
3. Verify the artifact upload step

---

**Happy Testing! 🎉**

*This demo shows how professional software development teams ensure code quality through automated testing.*
