# Basic Browser Sandbox (Demo)

This repository presents a **minimalist browser sandbox**, primarily intended as a **proof-of-concept and a straightforward demonstration** of embedding external web content within an `<iframe>` with basic sandboxing attributes. My goal was to create this entire sandbox within **a single file**, avoiding over-engineering and focusing purely on the core concept.

It's a quick example for local deployment and educational purposes, illustrating fundamental browser embedding capabilities and common limitations.

---

## Demo Video

See the sandbox in action by clicking the link below. The `demo.mp4` file is included directly in this repository in the `/assets` folder.

[Watch the Demo Video](./assets/demo.mp4)

---

## Features

* **URL Input**: Load external URLs into the sandbox.
* **Basic Iframe Embedding**: Utilizes a standard `<iframe>` for content.
* **`sandbox` Attribute**: Employs the `sandbox` attribute (`allow-scripts allow-forms allow-popups allow-pointer-lock allow-same-origin allow-top-navigation-by-user-activation`) for rudimentary control over embedded content.
* **Error Handling**: Basic detection of `X-Frame-Options` or `Content-Security-Policy` embedding restrictions.

---

## Limitations

As an advanced developer, please note the inherent limitations of this demo:

* **Security**: This sandbox provides only rudimentary isolation. It is **not suitable for securely Browse untrusted content** or any production environment requiring robust security.
* **X-Frame-Options/CSP**: Many modern websites actively prevent embedding via HTTP headers. This demo highlights these restrictions rather than attempting to bypass them.

---

## Getting Started

To run this demo locally, simply open the `index.html` file in your web browser. There are no server-side dependencies.

---

## License

This project is open-sourced under the MIT License.