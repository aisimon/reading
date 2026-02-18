## PR Reading

"Don't assume the data exists just because the feature is turned on. If the loading of data fails, you must explicitly catch that and handle it."

```php
public function processShipment(array $shipment)
{
    $isLocalCollect = isset($shipment['enhancements']['local_collect']);
    if ($isLocalCollect) {
        // 1. Attempt to load the data
        $locationData = $this->loadLocalCollectLocation($shipment);

        // 2. DEFENSIVE CHECK: Don't assume $locationData is valid 
        // just because $isLocalCollect is true.
        if (empty($locationData) || empty($shipment['pudo_location'])) {
            
            // 3. Explicitly catch the failure and handle it
            throw new \Exception(
                "You cannot use Local Collect without a valid pickup location. " .
                "Please check the pickup location of the shipment and try again."
            );
        }
    }
    // Only if we pass the validation above do we proceed to the carrier
    return $this->carrierApi->sendRequest($shipment, $locationData ?? null);
}
```
