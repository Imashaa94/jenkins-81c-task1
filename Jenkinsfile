// Declarative Pipeline for Part 1 – Task 1 (print-only design)

pipeline {
  agent any
  options { timestamps() }
  stages {
    stage('Build') {
      steps { echo 'TASK: Compile & package | TOOL: Maven' }
    }
    stage('Unit and Integration Tests') {
      steps { echo 'TASK: Run unit + integration tests | TOOLS: JUnit, Jest' }
    }
    stage('Code Analysis') {
      steps { echo 'TASK: Static code analysis | TOOL: SonarCloud (or ESLint)' }
    }
    stage('Security Scan') {
      steps { echo 'TASK: Dependency vulnerability scan | TOOL: npm audit (or Snyk)' }
    }
    stage('Deploy to Staging') {
      steps { echo 'TASK: Deploy app to staging | TOOL: SSH (or Ansible)' }
    }
    stage('Integration Tests on Staging') {
      steps { echo 'TASK: Run E2E/integration on staging | TOOL: Postman/Newman (or Cypress)' }
    }
    stage('Deploy to Production') {
      steps { echo 'TASK: Deploy app to production | TOOL: SSH (or Ansible)' }
    }
  }
}
