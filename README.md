# Scholarship Hub

Scholarship Hub is a responsive browser prototype for the Scholarship Management System requirements in `Requirements.docx`.

## Run it

Open `index.html` directly in a browser. No build step or server is required.

## Included flows

- Public scholarship discovery, search, catalog details, and eligibility checker
- Split student/admin authentication screens with client-side validation
- Student workspace with overview metrics, searchable catalog, four-step application form, document selection, application tracker, and profile editing
- Admin workspace with analytics, applicant search/sort/status filters, review actions, notes, document list, student directory, and scholarship add/edit/archive controls
- Role-based route guards that prevent student access to admin surfaces and admin access to student-only application pages
- MySQL-backed API integration through the standalone `backend/` service, with local demo data retained only as an offline fallback

### Demo administrator

Use `admin@scholarshiphub.test` with any password of at least eight characters.

The frontend calls `http://localhost:5000/api` by default. Start the backend and XAMPP MySQL before signing in. The API uses JWT authentication and server-side role checks. File metadata is stored by the API; production file storage still needs to be added.