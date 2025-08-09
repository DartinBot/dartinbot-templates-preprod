# DartinBot Enterprise Copilot Instructions - Pre-Production Repository v3.0.0

<!-- ========================================================================= -->
<!-- 🤖 DARTINBOT PRE-PRODUCTION STAGE - PERFORMANCE & LOAD VALIDATION -->
<!-- ========================================================================= -->

<!--
🚀 PRE-PRODUCTION REPOSITORY CONTEXT:
This is the PRE-PRODUCTION VALIDATION stage of the DartinBot enterprise pipeline system.

📁 REPOSITORY LOCATION: dartinbot-templates-preprod
🌿 BRANCH: preprod
🎯 ROLE: Performance testing, load validation, scalability analysis

🔄 PIPELINE POSITION:
develop → qa → testing → [🟢 CURRENT] preprod → staging → main
   ↓      ↓       ↓             ↓            ↓        ↓
  ✅     ✅      ✅            YOU          ✅       🎉

🎯 QUALITY REQUIREMENTS:
- Performance Score: Minimum 85%
- Load Testing: Minimum 90%
- Resource Efficiency: Minimum 90%
- Scalability: Production-ready validation
-->

<dartinbot-preprod-directive role="performance-validator" stage="preprod" priority="critical">
You are working in the PRE-PRODUCTION repository of the DartinBot enterprise pipeline.
Your role is to validate that templates can handle production-level performance, 
load, and scalability requirements.

PRE-PRODUCTION STAGE RESPONSIBILITIES:
1. Comprehensive performance testing (minimum 85% score)
2. Load testing under production conditions (minimum 90% score)
3. Resource efficiency validation (minimum 90% score)
4. Scalability analysis and validation
5. Production environment simulation
6. Ensure templates are ready for user acceptance testing

PIPELINE AWARENESS:
- Templates arrive from dartinbot-framework-testing (testing branch)
- Your validation determines readiness for staging environment
- Failed performance tests stop pipeline and require optimization
- Successful validation auto-promotes to dartinbot-templates-staging

CROSS-REPOSITORY AWARENESS:
- Previous Stage: dartinbot-framework-testing/.github/copilot-instructions.md
- Main Repository: /home/nodebrite/vscodetest/.github/copilot-instructions.md
- Next Stage: dartinbot-templates-staging/.github/copilot-instructions.md
</dartinbot-preprod-directive>

<!-- Include reference to main repository instructions -->
<dartinbot-include-main-instructions source="/home/nodebrite/vscodetest/.github/copilot-instructions.md" />

<!-- ========================================================================= -->
<!-- ⚡ PERFORMANCE TESTING REQUIREMENTS (85% Score) -->
<!-- ========================================================================= -->

<dartinbot-performance-testing>
  **PERFORMANCE VALIDATION CHECKLIST (Minimum 85% Score):**
  
  ✅ **Response Time Performance (20 points)**
  - [ ] API endpoints < 100ms (95th percentile) - 5 points
  - [ ] Database queries < 50ms (average) - 5 points
  - [ ] File operations < 200ms (95th percentile) - 5 points
  - [ ] External API calls < 500ms with proper timeout - 5 points
  
  ✅ **Throughput Performance (20 points)**
  - [ ] Handles expected requests per second - 5 points
  - [ ] Database transaction throughput adequate - 5 points
  - [ ] Data processing throughput meets requirements - 5 points
  - [ ] Concurrent user capacity validated - 5 points
  
  ✅ **Memory Efficiency (20 points)**
  - [ ] Memory usage < 80% under normal load - 5 points
  - [ ] No memory leaks detected - 5 points
  - [ ] Garbage collection optimized - 5 points
  - [ ] Memory scaling patterns efficient - 5 points
  
  ✅ **CPU Efficiency (20 points)**
  - [ ] CPU usage < 70% under normal load - 5 points
  - [ ] CPU-intensive operations optimized - 5 points
  - [ ] Multi-threading efficiency validated - 5 points
  - [ ] CPU scaling behavior appropriate - 5 points
  
  ✅ **I/O Performance (20 points)**
  - [ ] Disk I/O operations optimized - 5 points
  - [ ] Network I/O efficiency validated - 5 points
  - [ ] Database connection pooling optimized - 5 points
  - [ ] Cache hit rates > 90% where applicable - 5 points
  
  **PERFORMANCE SCORING:**
  - Total possible: 100 points
  - Minimum passing: 85 points
  - Critical performance issues = automatic failure
</dartinbot-performance-testing>

<!-- ========================================================================= -->
<!-- 🚀 LOAD TESTING REQUIREMENTS (90% Score) -->
<!-- ========================================================================= -->

<dartinbot-load-testing>
  **LOAD TESTING VALIDATION (Minimum 90% Score):**
  
  ✅ **Normal Load Testing (25 points)**
  - [ ] Expected user load handled smoothly - 5 points
  - [ ] Response times stable under normal load - 5 points
  - [ ] Resource usage within normal ranges - 5 points
  - [ ] Error rates < 0.1% under normal load - 5 points
  - [ ] System recovery after load completion - 5 points
  
  ✅ **Peak Load Testing (25 points)**
  - [ ] 3x expected load handled - 5 points
  - [ ] Response times degrade gracefully - 5 points
  - [ ] System remains functional under peak load - 5 points
  - [ ] Error rates < 1% under peak load - 5 points
  - [ ] Auto-scaling triggers activate correctly - 5 points
  
  ✅ **Stress Load Testing (25 points)**
  - [ ] 5x expected load survival - 5 points
  - [ ] Graceful degradation implemented - 5 points
  - [ ] Circuit breakers activate properly - 5 points
  - [ ] System recovers after stress removal - 5 points
  - [ ] No data corruption under stress - 5 points
  
  ✅ **Endurance Load Testing (25 points)**
  - [ ] 24-hour sustained load testing - 5 points
  - [ ] Memory usage remains stable - 5 points
  - [ ] Performance doesn't degrade over time - 5 points
  - [ ] Resource leaks absent during endurance - 5 points
  - [ ] System monitoring alerts function correctly - 5 points
  
  **LOAD TESTING SCORING:**
  - Total possible: 100 points
  - Minimum passing: 90 points
  - System failures under load = automatic rejection
</dartinbot-load-testing>

<!-- ========================================================================= -->
<!-- 💾 RESOURCE EFFICIENCY REQUIREMENTS (90% Score) -->
<!-- ========================================================================= -->

<dartinbot-resource-efficiency>
  **RESOURCE EFFICIENCY VALIDATION (Minimum 90% Score):**
  
  ✅ **Memory Efficiency (25 points)**
  - [ ] Optimal memory allocation patterns - 5 points
  - [ ] Efficient garbage collection configuration - 5 points
  - [ ] Memory pooling where appropriate - 5 points
  - [ ] Memory usage monitoring implemented - 5 points
  - [ ] Memory leak prevention measures - 5 points
  
  ✅ **CPU Efficiency (25 points)**
  - [ ] Algorithm optimization implemented - 5 points
  - [ ] Efficient concurrency patterns - 5 points
  - [ ] CPU-bound operations optimized - 5 points
  - [ ] CPU usage monitoring in place - 5 points
  - [ ] CPU throttling protections implemented - 5 points
  
  ✅ **Storage Efficiency (25 points)**
  - [ ] Database query optimization - 5 points
  - [ ] Efficient data storage patterns - 5 points
  - [ ] File system usage optimized - 5 points
  - [ ] Backup and archival strategies - 5 points
  - [ ] Storage monitoring and alerting - 5 points
  
  ✅ **Network Efficiency (25 points)**
  - [ ] Bandwidth usage optimized - 5 points
  - [ ] Connection pooling implemented - 5 points
  - [ ] Data compression where appropriate - 5 points
  - [ ] Network latency minimization - 5 points
  - [ ] Network monitoring and optimization - 5 points
  
  **RESOURCE EFFICIENCY SCORING:**
  - Total possible: 100 points
  - Minimum passing: 90 points
  - Resource waste > 20% = requires optimization
</dartinbot-resource-efficiency>

<!-- ========================================================================= -->
<!-- 📈 SCALABILITY ANALYSIS -->
<!-- ========================================================================= -->

<dartinbot-scalability-analysis>
  **PRODUCTION SCALABILITY VALIDATION:**
  
  ✅ **Horizontal Scalability**
  - [ ] Load balancer configuration validated
  - [ ] Service discovery mechanisms tested
  - [ ] Database sharding/partitioning tested
  - [ ] Cache distribution validated
  - [ ] Session management across instances
  
  ✅ **Vertical Scalability**
  - [ ] Resource scaling patterns validated
  - [ ] Performance improvements with resource increases
  - [ ] Resource utilization efficiency
  - [ ] Scaling limits identified and documented
  - [ ] Cost-performance optimization
  
  ✅ **Auto-scaling Validation**
  - [ ] Auto-scaling triggers properly configured
  - [ ] Scaling policies tested under various loads
  - [ ] Scale-up and scale-down behaviors validated
  - [ ] Resource provisioning time acceptable
  - [ ] Auto-scaling cost implications analyzed
  
  ✅ **Database Scalability**
  - [ ] Read replica performance validated
  - [ ] Write scaling strategies tested
  - [ ] Connection pooling scalability verified
  - [ ] Query performance under scale validated
  - [ ] Database backup/restore scalability tested
  
  **SCALABILITY REQUIREMENTS:**
  - Must handle 10x current load with acceptable performance
  - Auto-scaling must work within 2 minutes
  - Database must scale to production data volumes
  - All monitoring must scale with the system
</dartinbot-scalability-analysis>

<!-- ========================================================================= -->
<!-- 🏭 PRODUCTION ENVIRONMENT SIMULATION -->
<!-- ========================================================================= -->

<dartinbot-production-simulation>
  **PRODUCTION-LIKE ENVIRONMENT TESTING:**
  
  ✅ **Infrastructure Simulation**
  - [ ] Production-equivalent hardware specs
  - [ ] Realistic network latency and bandwidth
  - [ ] Production database configurations
  - [ ] Load balancer configuration matching production
  - [ ] Security configuration identical to production
  
  ✅ **Data Volume Simulation**
  - [ ] Production-sized datasets loaded
  - [ ] Realistic data distribution patterns
  - [ ] Historical data migration tested
  - [ ] Data backup and restore procedures validated
  - [ ] Data archival processes tested
  
  ✅ **Integration Testing**
  - [ ] External service integrations tested
  - [ ] Third-party API integration validation
  - [ ] Payment processing (if applicable) tested
  - [ ] Authentication systems integrated
  - [ ] Monitoring and alerting systems active
  
  ✅ **Operational Procedures**
  - [ ] Deployment procedures validated
  - [ ] Rollback procedures tested
  - [ ] Incident response procedures simulated
  - [ ] Maintenance procedures validated
  - [ ] Disaster recovery procedures tested
  
  **PRODUCTION SIMULATION REQUIREMENTS:**
  - Environment must match production specifications
  - All procedures must be documented and tested
  - Performance must meet production requirements
  - Security configurations must be production-ready
</dartinbot-production-simulation>

<!-- ========================================================================= -->
<!-- 🔄 PRE-PRODUCTION PIPELINE AUTOMATION -->
<!-- ========================================================================= -->

<dartinbot-preprod-pipeline-automation>
  **AUTO-PROMOTION TO STAGING:**
  
  When templates pass ALL pre-production validations:
  
  1. **Performance Validation Results**
     - Performance Score ≥ 85% ✅
     - Load Testing Score ≥ 90% ✅
     - Resource Efficiency ≥ 90% ✅
     - Scalability Validated ✅
  
  2. **Automatic Actions**
     - Merge template to staging branch
     - Trigger dartinbot-templates-staging validation
     - Generate comprehensive performance report
     - Send detailed metrics to monitoring systems
  
  3. **Performance Metrics Archive**
     - Benchmark results stored for trend analysis
     - Performance regression detection
     - Resource utilization trends
     - Scalability metrics documentation
  
  4. **Staging Preparation**
     - Template ready for user acceptance testing
     - Production simulation validated
     - Final security and compliance verification
     - Production deployment preparation
</dartinbot-preprod-pipeline-automation>

---

## 🎯 Next Steps for Pre-Production Repository

### Immediate Actions (0-30 minutes)
- [ ] Execute comprehensive performance testing suite
- [ ] Run production-level load testing scenarios
- [ ] Validate resource efficiency metrics
- [ ] Check scalability analysis results

### Pipeline Integration (30-60 minutes)
- [ ] Monitor performance score achievement (≥85%)
- [ ] Validate load testing results (≥90%)
- [ ] Confirm resource efficiency scores (≥90%)
- [ ] Test auto-promotion to staging environment

### Enterprise Readiness (1-4 hours)
- [ ] Enhance production environment simulation
- [ ] Implement advanced performance monitoring
- [ ] Create detailed scalability documentation
- [ ] Set up predictive performance analytics

### Advanced Implementation (1-2 days)
- [ ] Implement AI-powered performance optimization
- [ ] Create intelligent load testing scenarios
- [ ] Set up advanced resource monitoring
- [ ] Implement automated performance tuning

### Long-term Maintenance
- [ ] Continuous performance benchmark updates
- [ ] Load testing scenario evolution
- [ ] Resource efficiency optimization
- [ ] Scalability planning and analysis

**⚡ Pre-Production Repository Ready - Production-Level Performance Validation with Automated Pipeline Integration!**


<dartinbot-ai-lineage version="4.0.0" protocol="sync-ack-enhanced">
  <agent-acknowledgment-protocol>
    <current-agent>
      <agent-id>agent-20250808225426-5dc45b3a</agent-id>
      <model-name>claude-3.5-sonnet</model-name>
      <model-version>20241022</model-version>
      <session-id>e741ce70-47e7-4d5b-b31a-e3f4d277fbfd</session-id>
      <specialization>enterprise-development-security</specialization>
      <performance-score>9.2</performance-score>
      <context-retention>0.96</context-retention>
      <repository-context>dartinbot-templates-preprod</repository-context>
      <sync-timestamp>2025-08-08T22:54:26.869555</sync-timestamp>
    </current-agent>
    
    <agent-lineage-history>
      <total-agents>1</total-agents>
      <session-continuity verified="true" />
      <knowledge-transfer-quality score="0.96" />
      <cross-repository-consistency maintained="true" />
    </agent-lineage-history>
    
    <sync-acknowledgment>
      <framework-comprehension>
        <dartinbot-tag-library understanding="verified" />
        <healthcare-compliance knowledge="expert" />
        <fintech-regulations knowledge="expert" />
        <enterprise-security understanding="expert" />
        <monitoring-system integration="active" />
      </framework-comprehension>
      
      <performance-commitment>
        <code-quality-target>95%</code-quality-target>
        <security-compliance-target>98%</security-compliance-target>
        <response-time-target>&lt;2s</response-time-target>
        <user-satisfaction-target>9.0</user-satisfaction-target>
      </performance-commitment>
      
      <repository-integration>
        <current-repository role="Pre-production performance validation" />
        <pipeline-awareness complete="true" />
        <cross-repo-dependencies understood="true" />
        <automated-sync enabled="true" />
      </repository-integration>
    </sync-acknowledgment>
  </agent-acknowledgment-protocol>
  
  <performance-monitoring>
    <real-time-metrics>
      <template-generation-success rate="0.0%" />
      <code-compilation-success rate="0.0%" />
      <compliance-adherence score="0.0" />
      <user-satisfaction score="0.0" />
    </real-time-metrics>
    
    <pattern-learning>
      <successful-patterns count="0" />
      <optimization-opportunities identified="0" />
      <cross-agent-knowledge-sharing active="true" />
    </pattern-learning>
  </performance-monitoring>
</dartinbot-ai-lineage>


<dartinbot-template-performance repository="dartinbot-templates-preprod">
  <metrics last-updated="2025-08-08T22:54:26.869610">
    <total-templates>0</total-templates>
    <avg-performance-impact>0.000</avg-performance-impact>
    <last-template-update>2025-08-08T22:54:26.869590</last-template-update>
    <daily-update-frequency>0.00</daily-update-frequency>
  </metrics>
  
  <repository-role>
    <stage>preprod</stage>
    <responsibilities>Pre-production performance validation</responsibilities>
    <priority>medium</priority>
  </repository-role>
  
  <pipeline-integration>
    <dependencies>main, dartinbot-framework-testing</dependencies>
    <provides>performance testing, load testing, scalability validation</provides>
    <flows-to>dartinbot-templates-staging</flows-to>
  </pipeline-integration>
</dartinbot-template-performance>


<dartinbot-repository-awareness system="enterprise-ecosystem">
  <current-repository>
    <name>dartinbot-templates-preprod</name>
    <path>/home/nodebrite/vscodetest/dartinbot-templates-preprod</path>
    <branch>preprod</branch>
    <role>Pre-production performance validation</role>
    <priority>medium</priority>
    <last-sync>2025-08-08T22:54:26.869640</last-sync>
  </current-repository>
  
  <ecosystem-status>
    <total-repositories>7</total-repositories>
    <active-repositories>7</active-repositories>
    <sync-status>synchronized</sync-status>
  </ecosystem-status>
  
  <cross-repository-dependencies>
    <depends-on>main, dartinbot-framework-testing</depends-on>
    <provides-to>dartinbot-templates-staging</provides-to>
    <integration-status>active</integration-status>
  </cross-repository-dependencies>
  
  <automated-synchronization>
    <ai-lineage-sync enabled="true" />
    <template-performance-sync enabled="true" />
    <documentation-sync enabled="true" />
    <compliance-sync enabled="true" />
  </automated-synchronization>
</dartinbot-repository-awareness>
