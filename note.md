𝗝𝘂𝘀𝘁 𝗯𝘂𝗶𝗹𝘁 𝗮𝗻𝗱 𝗱𝗲𝗽𝗹𝗼𝘆𝗲𝗱 𝗮 𝗳𝘂𝗹𝗹𝘆 𝗺𝗼𝗱𝘂𝗹𝗮𝗿, 𝗽𝗿𝗼𝗱𝘂𝗰𝘁𝗶𝗼𝗻-𝗴𝗿𝗮𝗱𝗲 𝗔𝗪𝗦 𝗶𝗻𝗳𝗿𝗮𝘀𝘁𝗿𝘂𝗰𝘁𝘂𝗿𝗲 𝘂𝘀𝗶𝗻𝗴 𝗧𝗲𝗿𝗿𝗮𝗳𝗼𝗿𝗺 𝗮𝗻𝗱 𝗚𝗶𝘁𝗛𝘂𝗯 𝗔𝗰𝘁𝗶𝗼𝗻𝘀 𝗖𝗜/𝗖𝗗!🚀
This wasn’t just spinning up an EC2, hello no. I went full-stack on cloud infrastructure automation:

𝗣𝗿𝗶𝘃𝗮𝘁𝗲 𝗘𝗖𝟮𝘀 𝗯𝗲𝗵𝗶𝗻𝗱 𝗮 𝗽𝘂𝗯𝗹𝗶𝗰 𝗔𝗟𝗕 → No direct internet exposure. Only accessible through a NAT Gateway + ALB combo across multi-AZ subnets for high availability and secure traffic flow.

𝗔𝘂𝘁𝗼 𝗦𝗰𝗮𝗹𝗶𝗻𝗴 𝗚𝗿𝗼𝘂𝗽 (𝗔𝗦𝗚) → Automatically adjusts the number of EC2 instances based on CPU usage triggered from CloudWatch alarms, all launched via Launch Templates.

𝗠𝗼𝗱𝘂𝗹𝗮𝗿 𝗧𝗲𝗿𝗿𝗮𝗳𝗼𝗿𝗺 𝘀𝗲𝘁𝘂𝗽 → Clean, reusable modules for VPC, ALB, ASG, and web servers. Infrastructure is environment-specific with support for dev, staging, and prod.

𝗖𝗜/𝗖𝗗 𝘄𝗶𝘁𝗵 𝗚𝗶𝘁𝗛𝘂𝗯 𝗔𝗰𝘁𝗶𝗼𝗻𝘀 → Separate pipelines for each environment. Automated plan, validate, and apply workflows with secure GitHub secrets for AWS credentials.

𝗩𝗣𝗖 𝘄𝗶𝘁𝗵 𝗽𝘂𝗯𝗹𝗶𝗰/𝗽𝗿𝗶𝘃𝗮𝘁𝗲 𝘀𝘂𝗯𝗻𝗲𝘁 𝘀𝘁𝗿𝗮𝘁𝗲𝗴𝘆 → Includes Internet Gateway, NAT Gateway, route tables, and tight Security Group boundaries.

𝗟𝗶𝗻𝗸 𝘁𝗼 𝗥𝗲𝗽𝗼: https://lnkd.in/eYkRWbYf

⚠️ 𝗕𝗶𝗴𝗴𝗲𝘀𝘁 𝗰𝗵𝗮𝗹𝗹𝗲𝗻𝗴𝗲s?

 - 𝗖𝗲𝗿𝘁𝗶𝗳𝗶𝗰𝗮𝘁𝗶𝗼𝗻𝘀 = 𝗘𝘅𝗽𝗲𝗿𝗶𝗲𝗻𝗰𝗲→ Knowing the theory is one thing, but implementing real-world IaC was a whole different skill.
 - Handling state files and managing resources across environments without drift.

💜 𝗪𝗵𝗮𝘁 𝗜 𝗹𝗼𝘃𝗲𝗱 𝗮𝗯𝗼𝘂𝘁 𝗧𝗲𝗿𝗿𝗮𝗳𝗼𝗿𝗺
 - Clear infrastructure visibility
 - Reusability via modules
 - Rapid iteration via CI/CD

𝗡𝗲𝘅𝘁 𝘁𝗶𝗺𝗲: 
 - Add TFSEC or Checkov before terraform apply for security scanning.
 - Add Terratest for infra validation and bastion hosts for enhanced access control
 - Explore Secrets Manager for managing sensitive data

