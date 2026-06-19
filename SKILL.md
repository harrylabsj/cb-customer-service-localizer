---
skill: cb-customer-service-localizer
name: International Customer Service Localizer
type: descriptive
version: 1.1.0
description: Customer service adaptation for international audiences
author: Golden Bean (OpenClaw)
created: 2026-04-22
category: customer-service
language: en
tags: customer-service, localization, multilingual, support, international-operations
outputs: json
requires_api: false
safety_boundary: Descriptive cross-border e-commerce planning only. No code execution, API calls, network requests, bookings, or real-time data. Does not provide professional advice. Verify information with official sources and qualified professionals.
---

# International Customer Service Localizer

## Overview

International Customer Service Localizer (Customer service adaptation for international audiences). This skill provides a structured framework for localizing customer service operations for international markets. It covers multilingual support strategies, cultural service adaptation, channel selection, and quality management for cross-border customer service.

The framework helps businesses deliver culturally appropriate customer experiences across different markets while maintaining operational efficiency and service quality standards.

## Trigger Keywords

- "international customer service"
- "multilingual support localization"
- "cross-border customer experience"
- "global customer service strategy"
- "cultural service adaptation"
- "international support channels"

## Workflow

1. **Input Analysis**: Parse user input to extract target markets, service channels, and business parameters
2. **Localization Framework**: Generate culture-specific service adaptation recommendations
3. **Multilingual Planning**: Develop language support strategy and resource planning
4. **Channel Optimization**: Design market-appropriate service channels
5. **Output Delivery**: Return comprehensive JSON with analysis and recommendations

## Output Modules

### Service Localization Framework
- Communication style adaptation by culture
- Etiquette and protocol considerations
- Response time expectations by market
- Escalation process cultural adaptation
- Service recovery approach by culture

### Multilingual Support Plan
- Language coverage strategy and prioritization
- Translation vs localization approach
- Native speaker requirements and hiring
- AI and automation for language support
- Quality assurance for multilingual support

### Cultural Service Adaptation
- Greeting and opening style by culture
- Formality level adjustment recommendations
- Problem-solving approach by cultural context
- Complaint handling cultural differences
- Appreciation and follow-up cultural norms

### Channel Optimization
- Preferred support channels by market
- Social media customer service platforms
- Self-service portal localization
- Phone support cultural considerations
- Chat and messaging platform preferences

## Safety & Limitations

### Safety Boundaries
- **No Professional Advice**: Provides informational frameworks only. Does not replace HR or customer service professionals.
- **No Real-Time Data**: Based on general frameworks, not current staffing or platform availability.
- **No Service Delivery**: No actual customer service or support capabilities.
- **No Code Execution**: Pure descriptive implementation. No shell commands or network requests.
- **Descriptive Only**: Provides planning frameworks and guidance only.

### Limitations
- Cultural generalizations may not apply to all customer segments
- Language availability varies by market and changes over time
- Staffing costs and availability differ significantly by market
- Technology platform capabilities vary by region
- Service quality standards differ across cultures

## Example Prompts

### Level 1: Basic Inquiry
"How to localize customer service for international markets?"

### Level 2: Specific Scenario
"Multilingual support strategy for Japanese and German customers"

### Level 3: Complex Planning
"Multi-market customer service localization for US, EU, and Asia with omnichannel support"

### Level 4: Detailed Case
"US e-commerce company setting up customer service in France, Germany, and Japan with 24/7 multilingual chat support"

## Acceptance Criteria

### Functional Requirements
- Returns valid JSON structure from handle() function
- Includes input_analysis field with parsed input information
- Contains proper disclaimer with safety boundaries
- Provides customer-service-specific localization framework
- Differentiated from other cross-border e-commerce skills

### Quality Requirements
- Clear and structured output
- Comprehensive framework coverage
- Actionable implementation guidance
- Proper safety boundaries enforced
- Input differentiation verified through tests

## Integration

### Complementary Skills
- Works with cb-cultural-marketing-framework for consistent cultural approach
- Integrates with cb-returns-management-system for returns communication
- Supports cb-market-entry-strategist for market-specific service planning

### Input/Output Flow
- Accepts natural language input via handle() function
- Returns structured JSON for system integration
- Can be chained with related skills for multi-faceted analysis

## Version History

### v1.0.0 (2026-04-22)
- Initial release
- Service localization framework
- Multilingual support planning
- Cultural service adaptation
- Channel optimization guidance
- Input parsing and parameter extraction
- JSON output with input_analysis and disclaimer
- Safety boundaries and limitations documentation
- Test coverage with 5 tests per skill

## Technical Details

### Handler Interface


### Dependencies
- None (pure Python standard library only)

### File Structure
- handler.py: Main handler implementation
- tests/test_handler.py: Unit tests (5 tests)
- SKILL.md: This documentation file
- skill.json: Skill metadata and configuration
- ACCEPTANCE.md: Acceptance criteria documentation
- .claw/identity.json: Identity and authorship information

### Test Coverage
- JSON output validation test
- Disclaimer presence and content test
- Input differentiation test
- Customer-service-specific functionality test
- Differentiation evidence test


## Usage Scenarios

| # | User Input | Expected Output |
|---|---|---|
| 1 | "We offer email + chat support in English. We are launching in Japan. Redesign our support model for Japanese expectations." | Japan support model: add LINE as primary channel (expected by Japanese customers), phone support for complex issues (higher expectation than US), formal keigo-language templates, faster response SLA (Japanese customers expect <4 hours, not 24). Staffing: hire native Japanese team, not translation layer. |
| 2 | "Audit our localized support quality for the German market. We use a translation layer for English responses." | Quality audit: 50 ticket sample. Issues found: 30% have minor grammatical errors, 12% have incorrect formal/informal address (should use "Sie" not "du"), 5% have culturally inappropriate tone (too casual for complaint responses). Recommendation: native German support agents, not translation. |
| 3 | "Build a knowledge base localization playbook. We have 200 English articles - which to translate first, and how to adapt them for each market?" | Prioritization matrix: translate top 20 most-visited articles first (covers 65% of international traffic). Adaptation rules: Germany → add legal-disclaimer blocks; Japan → add visual step-by-step images (text-heavy = untrusted); Brazil → add WhatsApp share buttons. Localization budget estimate: $15K for Year 1. |


### Scenario 2: 海外客户投诉不知道怎么回
**User input:** "我们在亚马逊上卖产品，收到美国客户的差评说产品有质量问题。我们是中国人客服，不知道怎么用英文好好回复。"
**Expected output:** 亚马逊差评回复模板+本地化技巧——标准结构：1.感谢反馈+道歉（"Thank you for taking the time to share your experience. We sincerely apologize that the product did not meet your expectations."）；2.具体说明改进（"We have identified the issue with the battery life and our latest batch has been upgraded."）；3.提供补偿（"We'd love to make this right. Please contact us at [邮箱] for a full refund or replacement."）；4.表达长期承诺（"Your feedback helps us improve."）；常见差评类型模版：质量差→要求提供照片并退款、尺寸不符合→提供详细的测量指南退换货、送货慢→解释物流问题并给优惠券、功能类→给出详细使用教程+客服联系方式。关键：亚马逊差评回复要让其他潜在客户看到你的负责任态度而非只为让发差评的人满意。语气要诚恳+专业+行动导向。
