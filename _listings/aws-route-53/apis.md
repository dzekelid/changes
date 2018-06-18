---
name: AWS Route 53
x-slug: aws-route-53
description: Amazon Route 53 is a highly available and scalable cloud Domain Name
  System (DNS) web service. It is designed to give developers and businesses an extremely
  reliable and cost effective way to route end users to Internet applications by translating
  names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers
  use to connect to each other. Amazon Route 53 is fully compliant with IPv6 as well.Amazon
  Route 53 effectively connects user requests to infrastructure running in AWS &ndash;
  such as Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3
  buckets &ndash; and can also be used to route users to infrastructure outside of
  AWS. You can use Amazon Route 53 to configure DNS health checks to route traffic
  to healthy endpoints or to independently monitor the health of your application
  and its endpoints. Amazon Route 53 Traffic Flow makes it easy for you to manage
  traffic globally through a variety of routing types, including Latency Based Routing,
  Geo DNS, and Weighted Round Robin&mdash;all of which can be combined with DNS Failover
  in order to enable a variety of low-latency, fault-tolerant architectures. Using
  Amazon Route 53 Traffic Flow&rsquo;s simple visual editor, you can easily manage
  how your end-users are routed to your application&rsquo;s endpoints&mdash;whether
  in a single AWS region or distributed around the globe. Amazon Route 53 also offers
  Domain Name Registration &ndash; you can purchase and manage domain names such as
  example.com and Amazon Route 53 will automatically configure DNS settings for your
  domains.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Changes
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/aws-route-53/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Route 53 API Change Resource Record Sets
  x-api-slug: aws-route-53-api
  description: 'Create, change, update, or delete authoritative DNS information on
    all Amazon Route 53 servers.Send a POST request to:             /2013-04-01/hostedzone/Amazon
    Route 53 hosted ZoneID/rrset resource. The request body must include a document
    with aChangeResourceRecordSetsRequest element. The request body contains a list
    ofchange items, known as a change batch. Change batches are considered transactional
    changes.When using the Amazon Route 53 API to change resource record sets, Amazon
    Route 53 either makes all or none of thechanges in a change batch request. This
    ensures that Amazon Route 53 never partially implements theintended changes to
    the resource record sets in a hosted zone. For example, a change batch request
    that deletes the CNAME record forwww.example.com and creates an alias resource
    record set for www.example.com. Amazon Route 53 deletesthe first resource record
    set and creates the second resource record set in a singleoperation. If either
    the DELETE or the CREATE action fails, thenboth changes (plus any other changes
    in the batch) fail, and the original CNAMErecord continues to exist.ImportantDue
    to the nature of transactional changes, you can''t delete the same resourcerecord
    set more than once in a single change batch. If you attempt to delete the same
    changebatch more than once, Amazon Route 53 returns an InvalidChangeBatch error.NoteTo
    create resource record sets for complex routing configurations, use either thetraffic
    flow visual editor in the Amazon Route 53 console or the API actions for traffic
    policies andtraffic policy instances. Save the configuration as a traffic policy,
    then associate thetraffic policy with one or more domain names (such as example.com)
    or subdomain names (suchas www.example.com), in the same hosted zone or in multiple
    hosted zones. You can roll backthe updates if the new configuration isn''t performing
    as expected. For more information, seeUsing Traffic Flow to Route DNSTraffic in
    the Amazon Route 53 Developer Guide.Use ChangeResourceRecordsSetsRequest to perform
    the following actions:                  CREATE: Creates a resource record set
    that has the specified values.                  DELETE: Deletes an existing resource
    record set that has the specified values.                  UPSERT: If a resource
    record set does not already exist, AWS createsit. If a resource set does exist,
    Amazon Route 53 updates it with the values in the request. The values that you
    need to include in the request depend on the type of resource record set that
    you''re creating, deleting, or updating:            Basic resource record sets
    (excluding alias, failover, geolocation, latency, and weighted resource record
    sets)                           Name                                 Type                                 TTL                           Failover,
    geolocation, latency, or weighted resource record sets (excluding alias resource
    record sets)                           Name                                 Type                                 TTL                                 SetIdentifier                           Alias
    resource record sets (including failover alias, geolocation alias, latency alias,
    and weighted alias resource record sets)                           Name                                 Type                                 AliasTarget
    (includes DNSName, EvaluateTargetHealth, and HostedZoneId)                  SetIdentifier
    (for failover, geolocation, latency, and weighted resource record sets)When you
    submit a ChangeResourceRecordSets request, Amazon Route 53 propagates your changes
    to all of the Amazon Route 53 authoritative DNS servers. While your changes are
    propagating, GetChange returns a status of PENDING. When propagation is complete,
    GetChange returns a status of INSYNC. Changes generally propagate to all Amazon
    Route 53 name servers in a few minutes. In rare circumstances, propagation can
    take up to 30 minutes. For more information, see GetChange       For information
    about the limits on a ChangeResourceRecordSets request, see Limits in the Amazon
    Route 53 Developer Guide.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: ://///2013-04-01/hostedzone/Id/rrset/
  tags: Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/aws-route-53/20130401hostedzoneidrrset-post-openapi.md
- name: AWS Route 53 API Change Tags For Resource
  x-api-slug: aws-route-53-api
  description: Adds, edits, or deletes tags for a health check or a hosted zone.For
    information about using tags for cost allocation, see Using Cost Allocation Tags
    in the AWS Billing and Cost Management User Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: ://///2013-04-01/tags/ResourceType/ResourceId
  tags: Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/aws-route-53/20130401tagsresourcetyperesourceid-post-openapi.md
- name: AWS Route 53 API Get Change
  x-api-slug: aws-route-53-api
  description: 'Returns the current status of a change batch request. The status is
    one of thefollowing values:                  PENDING indicates that the changes
    in this request have not replicatedto all Amazon Route 53 DNS servers. This is
    the initial status of all change batchrequests.                  INSYNC indicates
    that the changes have replicated to all Amazon Route 53 DNSservers.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: ://///2013-04-01/change/Id
  tags: Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/aws-route-53/20130401changeid-get-openapi.md
- name: AWS Route 53 API
  x-api-slug: aws-route-53-api
  description: Amazon Route 53 is a highly available and scalable cloud Domain Name
    System (DNS) web service. It is designed to give developers and businesses an
    extremely reliable and cost effective way to route end users to Internet applications
    by translating names like www.example.com into the numeric IP addresses like 192.0.2.1
    that computers use to connect to each other. Amazon Route 53 is fully compliant
    with IPv6 as well.Amazon Route 53 effectively connects user requests to infrastructure
    running in AWS &ndash; such as Amazon EC2 instances, Elastic Load Balancing load
    balancers, or Amazon S3 buckets &ndash; and can also be used to route users to
    infrastructure outside of AWS. You can use Amazon Route 53 to configure DNS health
    checks to route traffic to healthy endpoints or to independently monitor the health
    of your application and its endpoints. Amazon Route 53 Traffic Flow makes it easy
    for you to manage traffic globally through a variety of routing types, including
    Latency Based Routing, Geo DNS, and Weighted Round Robin&mdash;all of which can
    be combined with DNS Failover in order to enable a variety of low-latency, fault-tolerant
    architectures. Using Amazon Route 53 Traffic Flow&rsquo;s simple visual editor,
    you can easily manage how your end-users are routed to your application&rsquo;s
    endpoints&mdash;whether in a single AWS region or distributed around the globe.
    Amazon Route 53 also offers Domain Name Registration &ndash; you can purchase
    and manage domain names such as example.com and Amazon Route 53 will automatically
    configure DNS settings for your domains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/aws-route-53/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/Route53/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/route53/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=87
- type: x-pricing
  url: https://aws.amazon.com/route53/pricing/
- type: x-registrar-policies
  url: https://aws.amazon.com/route53/amazon-registrar-policies/
- type: x-service-health
  url: http://status.aws.amazon.com/
- type: x-service-level-agreement
  url: https://aws.amazon.com/route53/sla
- type: x-sla
  url: https://aws.amazon.com/route53/sla/
- type: x-website
  url: https://aws.amazon.com/route53/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---