swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ReplaceNetworkAclAssociation:
    get:
      summary: Replace Network Acl Association
      description: Changes which network ACL a subnet is associated with.
      operationId: replacenetworkaclassociation
      x-api-path-slug: actionreplacenetworkaclassociation-get
      parameters:
      - in: query
        name: CidrBlock
        description: The IPv4 network range to allow or deny, in CIDR notation (for
          example                172
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Egress
        description: Indicates whether to replace the egress rule
        type: string
      - in: query
        name: Icmp
        description: 'ICMP protocol: The ICMP or ICMPv6 type and code'
        type: string
      - in: query
        name: Ipv6CidrBlock
        description: The IPv6 network range to allow or deny, in CIDR notation (for
          example                2001:bd8:1234:1a00::/64)
        type: string
      - in: query
        name: NetworkAclId
        description: The ID of the ACL
        type: string
      - in: query
        name: PortRange
        description: 'TCP or UDP protocols: The range of ports the rule applies to'
        type: string
      - in: query
        name: Protocol
        description: The IP protocol
        type: string
      - in: query
        name: RuleAction
        description: Indicates whether to allow or deny the traffic that matches the
          rule
        type: string
      - in: query
        name: RuleNumber
        description: The rule number of the entry to replace
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network ACL
  /?Action=ReplaceRouteTableAssociation:
    get:
      summary: Replace Route Table Association
      description: Changes the route table associated with a given subnet in a VPC.
      operationId: replaceroutetableassociation
      x-api-path-slug: actionreplaceroutetableassociation-get
      responses:
        200:
          description: OK
      tags:
      - Route Table