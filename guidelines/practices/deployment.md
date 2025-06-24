# Deployment specific suggestions

1. **Green continious testing in CI/CD:** 

   - Reduce automatic deployment to test or staging environments unless required. For instance, it might not be necessary when there's no meaningful change.
   - Single test execution per deployment cycle: Execute test cases only once during each deployment cycle, not on every module update.
   - Have a retention periods on test environment files so that even if you do nothing, they will disappear after a month or after three months or something.

2. **Reduce unnecessary deployments through batching:** Instead of deploying individual modules immediately after they're ready, bundle multiple changes and deploy on a fixed monthly schedule.

3. **Optimize CI/CD Build Efficiency with Parallelization:** Avoid running build and validation steps strictly in sequence. Instead, identify tasks that can run in parallel to reduce total processing time and energy consumption.

   > _Example: We managed to cut 30% of processing time used in the CICD build step._


4. **Audit and Minimize Deployment Package Size:** Regularly review deployment packages to eliminate unnecessary files or components. Smaller packages reduce transfer time, resource use, and energy consumed during deployment.

   > _Example: A deployment package was reduced from 630MB to 390MB, significantly cutting resource usage._

5. **Incorporate Energy Consumption Feedback into CI/CD Pipelines:** Integrate tools or scripts into your CI/CD pipeline to monitor and display energy consumption of builds and deployments. Developers can compare energy usage between versions and optimize based on real data.

6. **Visualize Energy Metrics for Developer Awareness:** Provide dashboards or pipeline feedback showing energy usage per build/deployment to raise awareness and support greener decisions during development.
   

