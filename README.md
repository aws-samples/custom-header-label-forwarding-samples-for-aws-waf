## How to use AWS WAF Bot Control for Targeted Bots signals and mitigate evasive bots with adaptive user experience

The [AWS WAF](https://aws.amazon.com/waf/) [Bot Control](https://aws.amazon.com/waf/features/bot-control/) rule group includes rules for detecting and managing bot threats. These threats range from easily identified common bots through to coordinated targeted bots that evade detection by operating across multiple hosts. Like any other security controls, Amazon Web Services (AWS) WAF Bot Control for Targeted Bots rules can also introduce ‘[false positives](https://aws.amazon.com/developer/application-security-performance/articles/managing-waf-false-positives-in-aws-waf/)’ that inadvertently prevent legitimate users to access the application. 

AWS WAF Bot Control for Targeted Bots rules use [Block, CAPTCHA, and Challenge](https://aws.amazon.com/blogs/networking-and-content-delivery/protect-against-bots-with-aws-waf-challenge-and-captcha-actions/) as the rule actions for mitigating bot threats based on indicators of bot activity. When it comes to protecting your web applications from bot threats, traditional methods such as blocking or CAPTCHA can often disrupt user experience. By default, Bot activity with a confidence signal of ‘high’ are blocked by AWS WAF, while CAPTCHA is used when there is uncertainty on whether the request is from a bot.

This git repository provides example webACL configurations for different mitigation strategies to adapt user experience using the forwarded signals as headers to your application. This way you can balance usability for legitimate users while also blocking evasive bots. Review the [post](https://aws-blogs-prod.amazon.com/networking-and-content-delivery/?p=25873&preview=true) for additional learning.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

