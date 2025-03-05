# hCaptcha 验证码解决方案

[![推广](https://github.com/bright-cn/LinkedIn-Scraper/raw/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://www.bright.cn/products/web-unlocker/captcha-solver/hcaptcha)

借助 Bright Data 先进的 CAPTCHA 解决技术，轻松绕过 hCaptcha 验证码。通过使用机器学习算法、[自动 IP 轮换](https://www.bright.cn/solutions/rotating-proxies)以及强大的代理基础设施，确保对目标站点的无缝稳定访问。  

Bright Data 的 CAPTCHA Solver 内置于 [**抓取浏览器**](https://www.bright.cn/products/scraping-browser) 和 [**网络解锁器 API**](https://www.bright.cn/products/web-unlocker) 中，为处理最复杂的验证码挑战提供完整解决方案。  

---

## 功能特性
- **高速验证码识别**：自动且快速地识别并解决 hCaptcha 验证码。  
- **IP 轮换**：通过自动重试和动态 IP 调整，避免 IP 封禁。  
- **浏览器指纹**：模拟真实用户行为，[绕过高级机器人检测](https://www.bright.cn/blog/web-data/anti-scraping-techniques)。  
- **JavaScript 渲染**：处理包含大量 JavaScript 动态内容的网站。  
- **全球地域覆盖**：精准解锁全球任意地区的内容。  
- **无缝集成**：可在 Puppeteer、Playwright、Selenium 等工具中轻松使用。  
- **事件监控**：跟踪验证码检测、成功或失败等事件。  

---

## 为什么选择 hCaptcha 验证码解决方案

### **全球 20,000+ 客户的信赖**  
Bright Data 的 CAPTCHA Solver 以高可靠性和高性能获得全球开发者、企业的广泛认可。  

### **基于高级代理网络**  
拥有超过 1 亿 IP 和先进的地理定位技术，强大的代理基础设施确保验证码的平稳解决过程。  

### **AI 驱动的验证码识别**  
我们的 CAPTCHA Solver 使用先进的 AI 逻辑自动检测、分析并解决验证码。它还能处理重试、指纹和请求头等方面，以绕过最复杂的反爬措施。  

### **针对开发者打造**  
- 与 Puppeteer、Playwright、Selenium 等轻松集成。  
- 完全可自定义的验证码解决策略。  
- 自动重试和动态 IP 调整，确保爬取不中断。  

> **专业提示 💡**  
>> 你已经拥有一套验证码解决方案？可搭配我们的 [Puppeteer](https://www.bright.cn/integration/puppeteer)、[Playwright](https://www.bright.cn/integration/playwright) 或 [Selenium](https://www.bright.cn/integration/selenium) 代理一起使用，进一步减少验证码出现的几率。

---

## 工作原理

Bright Data 的 CAPTCHA Solver 集成在 **Scraping Browser** 和 **Web Unlocker** 中，让验证码识别变得毫不费力。

### **自动处理验证码**  
CAPTCHA Solver 会实时检测并自动解决验证码。只需启用此功能，它将从检测到解决全过程自动处理。

#### 示例流程：
1. **检测验证码**：检测到验证码类型（如 hCaptcha）。  
2. **解决验证码**：利用 AI 逻辑完成验证码识别与解决。  
3. **失败重试**：若识别失败，系统会自动使用新 IP 重试。  
4. **返回结果**：验证码通过后，无缝访问目标网站。  

---

## 支持的验证码类型

Bright Data 的 CAPTCHA Solver 支持多种验证码类型，包括：

- [**DataDome**](https://www.bright.cn/products/web-unlocker/captcha-solver/datadome)
- [**reCAPTCHA**](https://www.bright.cn/products/web-unlocker/captcha-solver/recaptcha)
- [**Click Captcha**](https://www.bright.cn/products/web-unlocker/captcha-solver/click-captcha)
- [**hCaptcha**](https://www.bright.cn/products/web-unlocker/captcha-solver/hcaptcha)
- [**PerimeterX**](https://www.bright.cn/products/web-unlocker/captcha-solver/perimeterx)
- [**SimpleCaptcha**](https://www.bright.cn/products/web-unlocker/captcha-solver/simplecaptcha)
- [**FunCaptcha**](https://www.bright.cn/products/web-unlocker/captcha-solver/funcaptcha)
- [**Cloudflare Turnstile**](https://www.bright.cn/products/web-unlocker/captcha-solver/cloudflare-turnstile)
- [**AWS WAF Captcha**](https://www.bright.cn/products/web-unlocker/captcha-solver/aws-waf-captcha)
- [**GeeTest CAPTCHA**](https://www.bright.cn/products/web-unlocker/captcha-solver/geetest-captcha)
- [**KeyCAPTCHA**](https://www.bright.cn/products/web-unlocker/captcha-solver/keycaptcha)
- [**Puzzle CAPTCHA**](https://www.bright.cn/products/web-unlocker/captcha-solver/puzzle-captcha)
- [**Yandex CAPTCHA**](https://www.bright.cn/products/web-unlocker/captcha-solver/yandex-captcha)
- [**Image CAPTCHA**](https://www.bright.cn/products/web-unlocker/captcha-solver/image-captcha)
- [**Text CAPTCHA**](https://www.bright.cn/products/web-unlocker/captcha-solver/text-captcha)

---

## 高级自定义

[Bright Data CAPTCHA Solver](https://github.com/bright-cn/Captcha-solver) 提供高级自定义功能，可针对特定场景优化解决策略。

### **hCaptcha 挑战自定义配置示例**
```javascript
// 为不同验证码类型定义默认选项
function getCaptchaOptions(captchaType, customOptions = {}) {
  const defaultOptions = {
    timeout: 30000, // 等待验证码解决的最长时间（毫秒）
    check_timeout: 500, // 检查验证码状态的间隔（毫秒）
    wait_networkidle: { timeout: 1000 }, // 在网络空闲 1 秒后再进行下一步
    debug: false // 调试模式（默认关闭）
  };

  // 定义每种验证码的选择器
  const captchaSelectors = {
    DataDome: { selector: '#datadome-captcha', success_selector: '#captcha-success' },
    reCAPTCHA: { selector: '.g-recaptcha', success_selector: '.recaptcha-success' },
    ClickCaptcha: { selector: '.click-captcha', success_selector: '.captcha-passed' },
    hCaptcha: { selector: '.h-captcha', success_selector: '.hcaptcha-success' },
    PerimeterX: { selector: '#px-captcha', success_selector: '#px-success' },
    SimpleCaptcha: { selector: '.simple-captcha', success_selector: '.captcha-done' },
    FunCaptcha: { selector: '.funcaptcha', success_selector: '.funcaptcha-success' },
    CloudflareTurnstile: { selector: '.cf-turnstile', success_selector: '.cf-success' },
    AWSWAF: { selector: '#aws-waf-captcha', success_selector: '#aws-waf-success' },
    GeeTest: { selector: '.geetest-captcha', success_selector: '.geetest-success' },
    KeyCAPTCHA: { selector: '#keycaptcha', success_selector: '#keycaptcha-success' },
    PuzzleCAPTCHA: { selector: '.puzzle-captcha', success_selector: '.puzzle-solved' },
    YandexCAPTCHA: { selector: '#yandex-captcha', success_selector: '#yandex-success' },
    ImageCAPTCHA: { selector: '.image-captcha', success_selector: '.image-captcha-success' },
    TextCAPTCHA: { selector: '.text-captcha', success_selector: '.text-captcha-success' }
  };

  // 获取当前验证码类型对应的选择器
  const selectedOptions = captchaSelectors[captchaType] || {};

  // 合并默认配置、验证码类型选择器以及任何自定义覆盖
  return { ...defaultOptions, ...selectedOptions, ...customOptions };
}

// 不同验证码类型示例用法
const ddOptions = getCaptchaOptions('DataDome', { timeout: 40000, debug: true });
const recaptchaOptions = getCaptchaOptions('reCAPTCHA', { debug: true });
const hcaptchaOptions = getCaptchaOptions('hCaptcha');

console.log(ddOptions);
console.log(recaptchaOptions);
console.log(hcaptchaOptions);

// 示例错误处理
try {
  if (!document.querySelector(ddOptions.selector)) {
    throw new Error(`找不到验证码元素，使用选择器: ${ddOptions.selector}`);
  }

  // 在此处编写你的验证码解决逻辑
  solveCaptcha(ddOptions);
} catch (error) {
  console.error('验证码解决失败:', error.message);
}
```

---

## **事件监控**  
跟踪验证码解决事件，以处理高级用例：  
- `Captcha.detected`: 检测到验证码并开始解决。  
- `Captcha.solveFinished`: 验证码成功解决。  
- `Captcha.solveFailed`: 验证码解决失败。  

---

## **价格方案**

| **方案**          | **价格 (每 1000 个结果)** | **月度费用**       | **说明**                                  |
|-------------------|---------------------------|--------------------|-------------------------------------------|
| **按次付费**      | $1.50                    | 无固定承诺         | 适用于临时或小规模爬取需求。              |
| **成长型**        | $1.27                    | $499               | 专为需要扩展的团队而设计。                |
| **企业标准**      | $1.12                    | $999               | 适合大规模爬取的运营场景。               |
| **高级方案**      | $1.05                    | $1,999             | 高级功能与优先支持。                     |
| **企业定制**      | 按需定价                 | 联系我们           | 为大型企业提供定制化方案。               |

🚀 **特别优惠**：首次充值可享受最高可达 **$500** 的一倍匹配金额！

---

## **开发者喜欢 hCaptcha 验证码解决方案的原因**
- **易于集成**：可无缝应用于 Puppeteer、Playwright 和 Selenium。  
- **先进的 AI 识别逻辑**：自动处理重试、验证码解决、指纹、IP 轮换以及高级请求头。  
- **内置浏览器**：无需另行管理外部浏览器进行 JavaScript 渲染。  
- **实时洞察**：可通过实时仪表板监控网络性能。  
- **卓越支持**：全球 24/7 客户支持，且不断推出新功能。  

---

## **常见问题**

### **hCaptcha 验证码解决方案的原理是什么？**  
该解决方案使用先进的 AI 逻辑自动检测并解决 hCaptcha 验证码。  

### **它能同时处理多个验证码吗？**  
可以，该方案可扩展以同时处理多种验证码类型，保障访问不中断。  

### **如果验证码解决失败会怎样？**  
系统会自动进行重试。如问题持续存在，请联系我们 24/7 全天候客服以寻求帮助。  

---

## **告别 hCaptcha 验证码的烦恼**
立即开始免费试用，体验由 Bright Data 提供的无缝 [hCaptcha 验证码解决](https://www.bright.cn/products/web-unlocker/captcha-solver/hcaptcha)！
