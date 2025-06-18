// 6. Function to get form data
function handleGetFormData() {
    const nameElement = document.getElementById('name');
    const emailElement = document.getElementById('email');
    const cityElement = document.getElementById('city');
    const zipCodeElement = document.getElementById('zip-code');
    const statusElement = document.getElementById('status');
    if (!nameElement || !emailElement || !cityElement || !zipCodeElement || !statusElement) {
        console.error('One or more form elements are missing.');
        return null;
    }
    return {
        name: nameElement.value,
        email: emailElement.value,
        city: cityElement.value,
        zipCode: zipCodeElement.value,
        status: statusElement.checked
    };
}
