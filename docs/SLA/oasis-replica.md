# OASIS Replica Service Level Agreement

## Version Control
| *Version Number* | *Date* | *Author* | *Comments* |
| ---------------- | ------ | -------- | ---------- |
| 0.1 | 2-27-2013 | Scott Teige | First Draft |
| 0.2 | 3-28-2013 | Rob Quick | Revision of First Draft |

## Executive Summary
This SLA is an agreement between OSG Operations and the OSG Management and Stakeholders describing details of the OASIS software distribution system.

## Owners
This SLA is owned by OSG Operations and Indiana University and will be reviewed and agreed upon by the OSG Executive Team and OSG Stakeholders.

## Service Name and Description
### Name
OASIS (OSG Application and Software Installation Service) system
### Description

The OASIS service provides OSG Virtual Organizations with a central location for application software. The content hosted on OASIS can be made available on OSG compute resources. The service consists of three virtual machines, a stratum 0 CERN Virtual Machine File System (CVMFS) server, a stratum 1 replica of the stratum 0 and a node accessible for login by VO OASIS managers.

This SLA covers the stratum 1 replica. The stratum 0 and login SLA is available [here](/SLA/oasis.md).

## Security Considerations

The OASIS replica is accessible for login only by GOC and OSG technology group staff. It is publicly available as read-only.

## Service Target Response Priorities and Response Times

This section deals with unplanned outages. Please see [Requests for Service Enhancement](#requests-for-service-enhancements) for information on planned maintenance outages.

| Critical | High | Elevated | Normal |
| -------- | ---- | -------- | ------ |
| *Work Outage* | * * | * * | * * |
| The issue causes a full service or customer outage or a compromise to all stratum 1 replicas | The issue causes a full service outage or a compromise on the GOC replica instance | The issue causes short (less than 5 minute) periods of unstable or inconsistent performance | The issue causes minor (less than 10 seconds) periods of unstable or inconsistent performance |
| *Number of Clients Affected* | * * | * * | * * |
| The issue affects all replica users or OSG resources | The issue affects all replica users or OSG resources | The issue may or may not affect all replica users or OSG resources | The issue affects only a small number of replica users or OSG resources |
| *Workaround* | * * | * * | * * |
| All replicas are unavailable | replica failover mechanisms are used to direct usage away from the source of the outage | replica failover mechanisms are used to direct usage away from the source of the outage | No workaround will be necessary |
| *Response Time* | * * | * * | * * |
| Within one (1) hour | Workaround is addressed within (1) hour. Issue will be addressed by the next business day | Within the next business day | Within the next business day |
| *Resolution Time* | * * | * * | * * |
| The maximum acceptable resolution time is four (4) continuous hours, after initial response time | The maximum acceptable resolution time is 24 continuous hours, after the initial response time | The maximum acceptable resolution time is five (7) business days | The maximum acceptable resolution time is (30) business days |
| *Escalates Every* | * * | * * | * * |
| One Hour | Two Hour | One Day | One Week |

## Escalation Contacts

| *Escalation Level* | *OSG Contact* |
| ------------------ | ------------- |
| 1st | OSG Operations Infrastructure Lead |
| 2nd | OSG Operations Coordinator |
| 3rd | OSG Production Coordinator |
| 4th | OSG Technical Director and Executive Director |

Detailed information on contacts are viewable on the following [MyOSG URL](https://my.opensciencegrid.org/rgsummary/xml?summary_attrs_showhierarchy=on&summary_attrs_showservice=on&summary_attrs_showfqdn=on&summary_attrs_showcontact=on&gip_status_attrs_showtestresults=on&downtime_attrs_showpast=&account_type=cumulative_hours&ce_account_type=gip_vo&se_account_type=vo_transfer_volume&bdiitree_type=total_jobs&bdii_object=service&bdii_server=is-osg&start_type=7daysago&start_date=09%2F15%2F2009&end_type=now&end_date=09%2F15%2F2009&site_10047=on&rg=on&rg_336=on&gridtype=on&gridtype_1=on&active=on&active_value=1&disable_value=1), and are maintained within the

Any ongoing "Normal" or "Elevated" level issues will be discussed at the weekly [Operations](https://github.com/opensciencegrid/operations/tree/master/docs/WeeklyMinutes) and [Production](https://github.com/opensciencegrid/production/tree/master/docs/WeeklyMinutes) meetings.

## Service Availability and Outages

The GOC will strive for 99% service availability. If service availability falls below 99% monthly as monitored by the GOC on two consecutive months a root cause analysis and service plan will be submitted to the OSG stakeholders for plans to restore an acceptable level of service availability.

## Service Support Hours
The service is supported 24x7 by the GOC and Indiana University. All issues will be investigated by the next business day.

## Service Off-Hours Support Procedures
Users should contact the GOC via the [GOC trouble ticket](https://support.opensciencegrid.org) system.

## Requests for Service Enhancement

This section deals with planned maintenance outages. Please see [Service Target Response Priorities and Response Times](#service-target-response-priorities-and-response-times) for information on unplanned outages.

The OSG Operations will respond to customer requests for service enhancements based on GOC determination of the necessity and desirability of the enhancement. The GOC reserves the right to enhance the physical environment of the service based on IU and GOC needs. No enhancement will occur without advanced notice to the OSG community.

## Customer Problem Reporting
Service problems should be reported immediately by creating a problem ticket at <https://support.opensciencegrid.org>.

## Responsibilities
### Customer Responsibilities
OASIS customers agree to:

   * Use the service for purposes of OSG approved work only.
   * Alert the GOC if they are going to use the Service in a non-standard way, this includes testing or anticipated mass increases in usage.
   * Contact support by means outlined in the [Customer Problem Reporting](https://github.com/opensciencegrid/operations/blob/master/SLA/OASISServiceLevelAgreement#customer-problem-reporting) section of this document if they encounter any service issues.
   * Be willing and available to provide information within one business day for any High level issues reported.

### Responsibilities

GOC operations:
   * Maintain the physical machine hosting the service
   * Assure the service is accessible via its advertised URL
   * Make changes and updates within the normal GOC release schedule documented at https://github.com/opensciencegrid/operations/blob/master/SLA/ReleaseSchedule.
   * Meet response times associated with the priority assigned by users.
   * Maintain appropriately trained staff.

GOC Service Desk Responsibilities:
   * Log and track all Customer requests for service through the OSG ticketing system.

Database & Application Services responsibilities:
   * Announce and negotiate maintenance with stakeholders to assure minimal interruption to normal workload.
   * Alert the community of scheduled maintenance periods at least five (5) business days prior to the start of a service affecting maintenance window.

## Service Measuring and Reporting
The GOC will provide the customer with the following reports in the intervals indicated (monthly, quarterly, semi-annually, or annually):

| *Report Name* | *Reporting Interval* | *Delivery Method* | *Responsible Party* |
| ------------- | -------------------- | ----------------- | ------------------- |
| System Uptime | Monthly | Web Posting | GOC |
| Service Uptime | Monthly | Web Posting | GOC |
| Report of Critical and High Priority Issues | Quarterly | Web Posting | GOC |

These reports will be posted in Appendix E of this document.

## SLA Validity Period

This SLA will be in affect for one year.

## SLA Review Procedure

This SLA will renew automatically on a yearly basis unless change or update is requested by the OSG Operations Coordinator, the OSG Executive Team or the Stakeholders.

## References

# Appendix A - Customer Information
All service end-users who are members of an OASIS enabled VO and OSG Staff are considered customers.
Any VO can be OASIS enabled on request but it is anticipated that LHC associated VOs will use their existing CVMFS instances and will have no need for OASIS.

# Appendix B - Other Service Dependencies
The service is dependent on the following services to collect and distribute information:
   * Local Network and Hardware

# Appendix C - Supported Hardware and Software

## Supported Hardware
The following hardware is supported:
   * Physical devices used to provide the service.
   * Physical devices used to provide the environment used to house the service.

## Hardware Services
The following hardware services are provided:
   * Recommendations. OSG Operations will be responsible for specifying and recommending for purchase or lease hardware meeting customers' needs.
   * Installation. OSG Operations will install, configure and customize system hardware and operating systems.
   * Upgrades. OSG Operations is responsible for specifying and recommending for purchase any hardware upgrades.
   * Diagnosis. OSG Operations will diagnose problems with service related hardware.
   * Repair. OSG Operations analysts are not hardware technicians and receive no training in hardware maintenance, nor do we have the test equipment and tools necessary to do such work.

Performing repairs under warranty: Any work to be performed under warranty may be referred to the warranty service provider at the discretion of the Service Provider analyst(s). Service Provider analysts will not undertake work that will void warranties on customer hardware unless specifically requested and authorized by customer's management in writing.

Obtaining repair services: The Service Provider analyst will recommend a service vendor whenever he/she feels the repair work requires specialized skills or tools.

   * Backup. Service Provider agrees to fully back up all Service Provider-supported software and data nightly every business day.

## Software Services
Service Provider agrees to cover software support services, including software installations and upgrades. All software maintenance periods will be announced via the policy put forth in the [OSG Operations Responsibilities](#osg-operations-responsibilities) section of this document.

## Software Costs

IU and the Grid Operations Center bears all costs for new and replacement software contingent on the OSG Grant.

# Appendix D - Approval
| *Approved By* | *Position* | *Date* |
| ------------- | ---------- | ------ |
| | | |

# Appendix E - Metric Reports
   * [[ServiceLevelAgreements#Supporting_Documents][Recent availability statistics]]
