---
swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /factoryDevices/{factoryDeviceRef}:
    put:
      summary: Factory device update
      description: Updates the factory device corresponding to the provided factoryDeviceRef.
      operationId: updates-the-factory-device-corresponding-to-the-provided-factorydeviceref
      x-api-path-slug: factorydevicesfactorydeviceref-put
      parameters:
      - in: body
        name: device
        description: Contents of the factory device to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: factoryDeviceRef
        description: Ref of the factory device to update
      responses:
        200:
          description: OK
      tags:
      - Factory
      - Device
      - Update
  /asKeys/{asKeyRef}:
    put:
      summary: AS key update
      description: Updates the AS key corresponding to the provided asKey ref, if
        that AS key is within authorized scopes.
      operationId: updates-the-as-key-corresponding-to-the-provided-askey-ref-if-that-as-key-is-within-authorized-scope
      x-api-path-slug: askeysaskeyref-put
      parameters:
      - in: body
        name: asKey
        description: Contents of the AS key to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: asKeyRef
        description: Ref of the AS key to update
      responses:
        200:
          description: OK
      tags:
      - AS
      - Key
      - Update
---