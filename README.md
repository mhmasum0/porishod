# porishod

```mermaid
 graph TD;
    %% Onboarding & Login
    Start -->|Open App| SplashScreen
    SplashScreen -->|Proceed| LoginSignUp
    LoginSignUp -->|Enter Credentials| AccountVerification
    AccountVerification -->|OTP Verification| DashboardIntro
    DashboardIntro -->|First Time? Show Tutorial| LandlordDashboard
    
    %% Landlord Dashboard
    LandlordDashboard -->|View Properties| ManageProperties
    LandlordDashboard -->|View Payments & Requests| ManagePaymentsRequests
    LandlordDashboard -->|View Messages| ChatSupport
    LandlordDashboard -->|View Reports| FinancialReports
    LandlordDashboard -->|Logout| End
    
    %% Property & Apartment Management
    ManageProperties -->|Add Property| AddProperty
    AddProperty -->|Enter Details| PropertySelection
    PropertySelection -->|Enter Apartment Count| ListApartments
    ListApartments -->|Click Apartment| ApartmentDetails
    ApartmentDetails -->|Invite Tenant| InviteTenants
    InviteTenants -->|Send Email/SMS| TenantRegistration
    TenantRegistration -->|Tenant Registers| TenantManagement
    
    %% Tenant Management
    TenantManagement -->|View Applications| ApplicationManagement
    ApplicationManagement -->|Approve/Reject| ApproveReject
    
    %% Rent & Utility Payment Management
    ManagePaymentsRequests -->|Set Rent & Bills| SetRentBills
    SetRentBills -->|Track Payments| PaymentTracking
    PaymentTracking -->|Send Reminders| PaymentReminder
    
    %% Chat and Communication
    ChatSupport -->|List Conversations| ChatDashboard
    ChatDashboard -->|Send Messages| ChatInterface
    
    %% Maintenance Requests
    LandlordDashboard -->|Manage Maintenance| ServiceRequests
    ServiceRequests -->|View Issue| IssueDetails
    IssueDetails -->|Update Status| StatusManagement
    
    %% Lease & Document Management
    LandlordDashboard -->|Manage Leases| LeaseManagement
    LeaseManagement -->|Upload Lease| UploadDocuments
    UploadDocuments -->|Send for Signature| DigitalSignature
    DigitalSignature -->|View Repository| DocumentRepository
    
    %% Tenant App Flow
    UserType -->|Tenant| TenantDashboard
    TenantDashboard -->|View Rent Due| PaymentPortal
    PaymentPortal -->|Make Payment| PaymentConfirmation
    PaymentPortal -->|Setup Auto-Payment| AutoPayment
    TenantDashboard -->|View Statements| StatementAccess
    StatementAccess -->|Download Invoices| InvoiceDownload
    TenantDashboard -->|Request Maintenance| MaintenanceRequests
    MaintenanceRequests -->|Submit Request| RequestTracking
    RequestTracking -->|Chat with Service| ServiceChat
    TenantDashboard -->|Chat with Owner| TenantChat
    TenantChat -->|Send Messages| TenantMessaging
    TenantDashboard -->|View Lease| LeaseAccess
    LeaseAccess -->|Sign Digitally| LeaseSignature
    LeaseAccess -->|Download Copy| LeaseDownload

```
